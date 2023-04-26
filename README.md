# Fiverr-GPT-content-creator

To install the program:

git clone https://github.com/salomonsa/Fiverr-GPT-content-creator.git

IMPORTANT STUFF, READ BEFORE USING THE PROGRAM:

1. Change the name of the env-example file to .env, open it and write your OPENAI API token, your desired mail with its password in their respective variables.

2. Install all the requirements in the requirements.txt file. Also, and this is ESSENTIAL for the program to work, install separately Imagemagick in its official website. If there's an error regarding ImageMagick while using the program and ImageMagick is installed in your computer, you must rewrite the following line of code in main.py: change_settings({"IMAGEMAGICK_BINARY": r"C:/Program Files/ImageMagick-7.1.1-Q16-HDRI/magick.exe"}) to the following change_settings({"IMAGEMAGICK_BINARY": r"{Directory in which you've installed ImageMagick}/magick.exe"}) replacing accordingly what's inside the curly brackets.

3. Before using the program, I recommend you to first try to upload a video manually with the Youtube account you'll use. This is recommendable because the first time one uploads a Youtube video there might be certain pop-ups which could interrupt the process of uploading the video and therefore making the program fail.

4. If there is any error regarding the upload of the video or the Youtube Sign in, you can go to the upload.py and change the following line of code in the 2 functions: browser = playwright.firefox.launch(headless=False) to browser = playwright.firefox.launch(headless=True). This will allow you to see directly which part of the process is failing exactly. Once you've detected the error, you can change the lines of code to what they were before.

5. If you want to change the amount of minutes the program waits between finishing the upload of a video and starting to generate and upload the next one, you can go to the variable minutes in the main.py file and change it there (it is a float so decimals are allowed).

6. Create the following 3 folders on your directory: music, video, data. Put inside the music and video folders the music and videos you want to use. Never delete the data folder.

7. All videos, titles, descriptions and tags are saved in the output folder, each on their own folder following the name pattern Folder1, Folder2, etc. Inside each of these folders, like Folder1 for example, there will be the following: video.mp4 title.txt description.txt and tags.txt each representing their respective attributes according to their file names.

8. The language set to the Google account you're using must be english, so change it if you have any other language on.

9. Just tell me if there's anything not going well or lacking! :)
