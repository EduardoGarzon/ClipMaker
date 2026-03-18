# Description of Application Development
This web application was developed based on essential web development and programming logic principles, using technologies such as HTML, CSS, JavaScript, and Tailwind CSS to build the interface. Furthermore, it integrates external services through APIs, notably the use of Cloudinary for video upload and processing, and the Gemini API for applying Artificial Intelligence to transcript analysis.

Development was carried out using Visual Studio Code with support from GitHub Copilot, which enabled greater productivity and guided learning. Initially, fundamental HTML concepts were explored, such as structuring with tags and attributes, and the use of CSS for styling and creating modern layouts. Then, JavaScript was introduced to add interactivity to the application, covering DOM manipulation, functions, conditionals, and events.

In the next stage, integration with Cloudinary was implemented, allowing video uploads and the use of automated workflows for transcript generation. This process was essential to enable the analysis of video content.

Finally, integration with the Google Gemini API was implemented, which is responsible for analyzing the generated transcript. The application sends a POST request containing the transcript and a structured prompt, asking the AI ​​to identify the segment with the greatest viral potential. In response, Gemini returns the start and end timestamps of the most relevant moment in the video.

***

# Application Operation

### The workflow is as follows:

1. The user uploads a video through the interface.

2. The video is sent directly to Cloudinary.

3. A pre-configured workflow automatically generates a transcript of the content.

4. The transcript is sent to Gemini via a POST request.

5. The AI ​​analyzes the text and returns the start and end times of the most viral segment.

6. Based on this data, the application builds a dynamic Cloudinary URL containing only the video clip.

7. The final clip is displayed directly in the user interface.

***

This project demonstrates, in practice, the integration between modern frontend development, cloud services, and Artificial Intelligence. Furthermore, it reinforces the importance of understanding how APIs work, good programming practices, and building complete applications, from the interface to data processing.

***

# Application Interface
<img width="1708" height="851" alt="Imagem_da_Interface" src="https://github.com/user-attachments/assets/83a4e29a-8bc5-4919-9cf6-68aefbcacf65" />

***

# Demonstration Video

The video used as an example is about 5 minutes long and discusses what the JavaScript language is. The application analyzes this content and automatically returns a clip between 30 and 60 seconds long, corresponding to the segment with the highest viral potential identified by the AI.

https://github.com/user-attachments/assets/824b7789-e3ba-484d-a198-3caf4b567c0b
