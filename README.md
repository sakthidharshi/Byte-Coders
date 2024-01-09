# Byte-Coders 
-- Create a database
CREATE DATABASE IF NOT EXISTS indic_language_database;
USE indic_language_database;

-- Create a table with support for Indic languages
CREATE TABLE indic_data (
    id INT PRIMARY KEY AUTO_INCREMENT,
    text_content TEXT CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci,
    language_code VARCHAR(10)
);

-- Insert sample data
INSERT INTO indic_data (text_content, language_code) VALUES
('नमस्ते कैसे हैं', 'hi'), -- Hindi
('আপনি কেমন আছেন', 'bn'), -- Bengali
('வணக்கம் எப்படி உள்ளீர்கள்', 'ta'); -- Tamil

-- Query data
SELECT * FROM indic_data;
