# PhotosPreprocessing
If you are a photographer then you can faced problem when you need to manually rotate wrongly rotated photos and to delete blury photos. This solution do all work instead of you!

My solution automatically moves blury ptohos and then rotates photos to the right angle

# How to use
1. Clone the repository
2. IMPORTANT: Download model from: https://drive.google.com/file/d/1GjUsPt6uMCjfQwy7GKgKaK-ojjMhKIcr/view?usp=sharing
3. Start the program like:
   python FolderProcess.py --folder C:\Photos\MY_FOLDER --device cpu --out C:\Good_Photos --blur C:\Bad_Photos --threshold 13 --model ./best_model_resnet50_acc99.pth', help='Location to state_dict of the model .pth

# Arguments:
--device ("cpu" or "cuda", default="cpu"): If your GPU does not support CUDA, then choose "cpu"
--threshold (default=13): Blur threshold to determine blury images. Higher value means better quality of selection
--out: Loacation to folder where rotated and quality photos will be stored
--blur: Location to folder, where blury photos will be stored
--folder: Folder which contains yout photos to proceed
--model: Location to state_dict of the model .pth
