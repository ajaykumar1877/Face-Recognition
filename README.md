📌 Face Recognition with OpenCV & face_recognition
Description

This project demonstrates a face recognition system using the face_recognition library (built on dlib) along with OpenCV for image handling.

🚀 Workflow

Image Reading & Preprocessing

Each image is resized proportionally for faster processing.

Encoding Known Faces

All images in the known/ folder are loaded.

For each face, a 128-d embedding is generated using face_recognition.face_encodings().

Encodings and corresponding names are stored.

Testing Unknown Faces

Images from the unknown/ folder are processed.

The face embeddings are compared against the known encodings using compare_faces().

Annotation

If a match is found, the face is bounded with a rectangle.

The identified person’s name is displayed above the face.

Output

Displays the recognized faces with labels.
