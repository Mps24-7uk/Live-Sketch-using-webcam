# Live-Sketch-using-webcam

The Goal this project is make live sketch using computer vision.

# Dependencies

1. Opencv

# Step by Step Explanation

1.  Read the Live vedio by using videocapture
2.  To remove complexity, Convert the frame using cv2.cvtColor(image, cv2.COLOR_BGR2GRAY) 
3.  To remove noise,convert the frame cv2.GaussianBlur(img_gray, (5,5), 0)
4.  To extract the edges cv2.Canny(img_gray_blur, 10, 70) is used
5.  To display the live-sketch cv2.threshold(canny_edges, 70, 255, cv2.THRESH_BINARY_INV) is used  
