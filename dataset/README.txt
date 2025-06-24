# CCTV Face Detection Dataset

This dataset is designed for training and evaluating computer vision models in face detection and re-identification tasks within CCTV-like environments.

## 📁 Directory Structure

```
dataset_split/
├── train/
│   ├── images/
│   │   ├── face_0001.jpg
│   │   └── ...
│   └── labels.csv        # includes: filename, emp_id
├── test/
│   └── images/
│       ├── face_1250.jpg
│       └── ...
├── reference_faces/
│   ├── emp001/
│   │   ├── face1.jpg
│   │   └── face2.jpg
│   └── ...
```

### ✅ Train Folder

Contains:

- `images/`: Cropped face images used for training.
- `labels.csv`: Metadata file with the following format:
  ```
  id,filename,emp_id
  face_0001.jpg,emp001
  face_0002.jpg,emp002
  ...
  ```

### ✅ Test Folder

Contains:

- `images/`: Cropped face images used for testing.
- ⚠️ `labels.csv` is **intentionally removed** to simulate realistic evaluation settings such as Kaggle competitions. Ground truth is held privately by the competition organizers.

### ✅ Reference Faces

The `reference_faces/` directory contains:

- Subfolders named by anonymized employee IDs (`emp001`, `emp002`, etc.)
- Each subfolder includes multiple high-quality, clear facial images of the respective employee.

These can be used as a **gallery** for recognition or embedding comparison tasks.

---

## 🔒 Privacy

All identities are anonymized using consistent numeric employee codes (e.g., `emp001`, `emp002`, ...), ensuring privacy and confidentiality.

## 📚 Usage

This dataset is ideal for:

- Training face detection and identification models
- Performing face re-identification using reference images
- Benchmarking cropped face-based recognition workflows

---