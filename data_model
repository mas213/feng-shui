# 🌊 Windsurf App – Data Model (ERD in Markdown)

## 1. Users

- `id` (UUID, PK)
- `name` (String)
- `email` (String, unique)
- `password_hash` (String)
- `profile_photo_url` (String, optional)
- `experience_level` (Enum: Beginner, Intermediate, Advanced)
- `created_at` (Timestamp)
- `updated_at` (Timestamp)

## 2. Gear

- `id` (UUID, PK)
- `user_id` (UUID, FK → Users.id)
- `type` (Enum: Board, Sail, Mast, Boom, Fin)
- `brand` (String)
- `model` (String)
- `year` (Integer)
- `size` (String or Float, e.g. "6.0m²", "115L")
- `notes` (Text, optional)
- `is_active` (Boolean)
- `created_at` (Timestamp)

## 3. Spots

- `id` (UUID, PK)
- `name` (String)
- `location` (String or Coordinates)
- `country` (String)
- `best_season` (String)
- `difficulty_level` (Enum: Easy, Moderate, Challenging)
- `spot_type` (Enum: Lake, Ocean, Bay, River)
- `description` (Text)
- `thumbnail_url` (String)
- `created_by_user_id` (UUID, FK → Users.id)
- `created_at` (Timestamp)

## 4. Sessions

- `id` (UUID, PK)
- `user_id` (UUID, FK → Users.id)
- `spot_id` (UUID, FK → Spots.id)
- `date` (Date)
- `start_time` (Time)
- `end_time` (Time)
- `wind_avg_knots` (Float)
- `wind_gust_knots` (Float)
- `conditions_description` (Text)
- `gear_ids` (Array[UUID], FK → Gear.id)
- `notes` (Text, optional)
- `rating` (Integer, 1–5)
- `created_at` (Timestamp)

## 5. WeatherSnapshots (optional if pulling from API)

- `id` (UUID, PK)
- `spot_id` (UUID, FK → Spots.id)
- `timestamp` (Timestamp)
- `wind_speed_knots` (Float)
- `wind_direction_deg` (Integer)
- `temperature_celsius` (Float)
- `weather_condition` (Enum: Sunny, Cloudy, Rainy, Stormy, etc.)
- `wave_height_m` (Float)
- `tide` (String)
- `data_source` (String, e.g. "WindyAPI", "NOAA")

---

## Relationships

- A `User` can own multiple `Gear` items.
- A `User` can log multiple `Sessions`.
- Each `Session` is associated with one `Spot`.
- A `Session` can use multiple `Gear` items (many-to-many via array or pivot table).
- `Spots` can be created by users and are shared.
- `WeatherSnapshots` are optional but enrich session and spot data.

