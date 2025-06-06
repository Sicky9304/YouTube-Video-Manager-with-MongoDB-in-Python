
# 🎥 YouTube Video Manager

A Python-based command-line application to manage YouTube video records using MongoDB. Supports adding, viewing, searching, updating, and deleting video metadata.

---

## 📁 Files

- `youtube manager.py` – Main Python script for managing video entries.
- MongoDB Database: `YouTube`
- Collection: `youtube_manager`

---

## 🛠 Features

- ✅ Insert new video details
- ✅ View all stored video records
- ✅ Search for videos by title (partial match supported)
- ✅ Update video information by ID
- ✅ Delete video record by ID
- ✅ MongoDB integration for persistent storage

---

## 💻 How to Run

1. **Ensure MongoDB is installed and running locally**  
   [Install MongoDB](https://www.mongodb.com/try/download/community)

2. **Install Python dependencies (if not already installed)**

   ```bash
   pip install pymongo
   ```

3. **Run the Python script**

   ```bash
   python "youtube manager.py"
   ```

---

## 🧪 Example Usage

```
Welcome to YouTube Video Manager
1. Insert Video
2. View Videos
3. Search Video
4. Update Video
5. Delete Video
6. Exit

Enter your choice: 1
Enter the video ID: 1001
Enter the Video title: How to Learn Python
Enter the video description: Beginner Python Tutorial
Enter video category: Education
Enter upload date(YYYY-MM-DD): 2025-06-06
Video inserted with ID: 1001
```

---

## 📦 MongoDB Document Format

Each video is stored as:

```json
{
  "_id": 1001,
  "title": "How to Learn Python",
  "description": "Beginner Python Tutorial",
  "category": "Education",
  "upload_date": "2025-06-06"
}
```

---

## 🔒 Notes

- Ensure that MongoDB is running on `localhost:27017`.
- `_id` must be unique for each video.
- All user inputs are taken from the terminal (CLI-based interface).

---

## 📄 License

This project is free for personal and educational use.
