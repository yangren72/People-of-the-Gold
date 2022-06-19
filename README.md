# People of the Gold
### by Yang Ren (2022)
<br>

[website link](https://yangren72.github.io/People-of-the-Gold/website/)
<br><br>

#### Artist Statement:

"People of the Gold" is a project that reflects on the identity, and history of the early Chinese immigrants in California during the period of Gold Rush. The project consists of multiple archive-looking moving images generated by a machine learning algorithm trained with historical documents. The work is presented in a minimalistic interface for viewer to browse. The constantly changing portrait photo of people and the "identity information" next to the photos are presented. Viewers are invited to browse those files slowly, replicating the experience of browsing historical documents. The project aims to raise awareness and emotions to the history of those people of the gold through exploring the potential of machine learning algorithm in the field of photographic imaging and anthropology studies.

I first get the images from my [source](https://digitallibrary.californiahistoricalsociety.org/object/22481?solr_nav%5Bid%5D=74504d2e9f0c5c063c30&solr_nav%5Bpage%5D=2&solr_nav%5Boffset%5D=9#page/1/mode/2up). I input the images into lightroom to adjust the cropping, background, and resolution to prepare them for Ml training. I use StyleGan-2-ada with Pytorch to train my two models, one focuses on the portrait, the other focuses on the archive file. The instructions and the code, I take reference from [Jeff Heaton](https://github.com/jeffheaton) and [NVIDIA](https://github.com/NVlabs/stylegan2-ada-pytorch) I run the training on google colab. Later I explored the latent space and downloaded the generated image sequences. I then put the images into the after effect and combined the two videos(portraits and archive) together. I wrote a website with HTML and CSS to present the video loop.

I trained my models on the Google Colab virtual machine. The code is a bit hard to show. So I decided to put two python files in Github that contain the code I use for Training and for Generation.

Machine learning is a big part of the project in terms of techniques. However, it is seen by me as a creative tool to open more possibilities of image making, rather than problem solving. I read an article a few months ago talking about the Chinese immigrants in the early 1900s. I also found the database of the archive files. The history immediately interested me. After I learned about machine learning in the class, I came up with an idea of using the machine learning tool to create a generative program that can generate faces. The ML model directly learns from the real images and uses its "magic" to combine the details of people's faces together to create a new portrait. This process is fascinating when thinking about it in a photographic way. I see this as a special form of group portrait. It is like a photo collage, but arguably more random (less human interference) but also very smooth. When Interpolating the latent space, the transitions of the millions of faces and information inside it gives me a sense that it is bigger than life. It is bigger than individuals. It feels like it holds the spirit of the people in the past. It holds the spirit of history.

The reason I choose to present it in a way of the archive file is that when it is presented with the archive files style image, the people are generalized with the format. The individuality is decreased and the sense of a group of people is strengthened. The viewers are distanced, which makes people think more about the history aspect of the story instead of a more personal one. I think it is more calm but profound.

The piece is present in a minimalistic website that has a simple interface of viewing. The archive style files are layout in the main page. All of the archive style files are moving slowly. The viewer can click on the small image to open up the image for a closer detailed look. The website is dark and clean, to replicate the feeling of browsing and trying to find the historical files. The interfaces are designed to allow the viewers to slowly look at whichever they prefer to look in whatever order they want. Each video loop is unique and the movement is quite slow forcing the viewer to calm down and look into the details just as what we do when we are looking into objective historical documents.

