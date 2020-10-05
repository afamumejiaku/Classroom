CS 5331-002 - Virtual Reality Project 1
Due: October 4, 2020
Project Report
I learned...
•	The basics of Three.js and A-Frame
•	How the Document Object Model works (DOM)
•	Front-end design techniques that greatly take into consideration UX
•	How to manipulate 3-D .gltf models using blender
•	General JavaScript library usage
•	How to use Chrome's web development tools
•	The meta of WebVR and the existence of cool online virtual reality applications
Biggest issues
•	I was mostly worried about my scene not running smoothly on a mobile device. To compensate for this I made sure to add means of moving in mobile scences and removed all downloaded materials
•	Library collision - certain libraries set contradictive variables within one another and this would cause problems with the applications as a whole. For example, the A-Frame Extras Plugin would instantiate movement controls that were supported on a desktop but not on a mobile phone.
Contributors
•	Individual project; All work was completed by Umejiaku Afamefuna.
Work Distribution
________________________________________
In the JavaScript functions explained below, the following global variables (declared in the HTML head) are used to enable play and pause for both the video and audio.
 AFRAME.registerComponent('play', {
        init: function () {
          var myEl = document.querySelector('#man')
          this.el.addEventListener('click', function () {
            myEl.components.sound.playSound()
          })
        },
      })
    </script>

    <script>
      AFRAME.registerComponent('play-pause', {
        init: function () {
          var myVideo = document.querySelector('#lectures')
          var videoControls = document.querySelector('#videoControls')
          this.el.addEventListener('click', function () {
            if (myVideo.paused) {
              myVideo.play()
              videoControls.setAttribute('src', '#pause')
            } else {
              myVideo.pause()
              videoControls.setAttribute('src', '#play')
            }
          })
        },
      })
    </script>
Key features

Dynamic features/interactables
Dynamic features include the windows, doors the lecture among others.

I have designed all the items in the project. They include the 
1. Class Chairs
2. Class Tables
3 Lecturers desk
4.Fan
5. Lecture
6. computer
7. street Light
8. Traffic Light
9. The Wall Frames
10. Buildings
Among others in the scene.

