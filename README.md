# Welcome to My Moving Box Realtime
***

## Task
- The problem was writng a javascript code in order to move the "div" with the id my_box_realtime to the coordinates of bottom: 0 and right 0. Moving the box must be smooth. This means you will update the position slowly: You can only change the position (vertically and horizontally) by 1 point every 0.5 seconds.

## Description
- Though the excerses were challenging at first but i was to solve it with the help of the videos, my peers and with  help of google research.


        #my_box_realtime {
            background-color: red;
        }
        #my_box_realtime {
            position: absolute;
        }
        #my_box_realtime {
            right: 70px;
        }
        #my_box_realtime {
            bottom: 70px;
        }
        #my_box_realtime {
            min-width: 100px;
        }
        #my_box_realtime {
            min-height: 100px;
        }
        #my_box_realtime {
            transition: all 0.5s linear;
        }

>
    <div id="my_box_realtime"></div>
    <script type="text/javascript">
        const box = document.getElementById('my_box_realtime');
        const screenWidth = window.innerWidth;
        const screenHeight = window.innerHeight;

        let xPos = 70; 
        let yPos = 70; 

        const moveBox = () => {
            if (xPos < screenWidth - 100 && yPos < screenHeight - 100) {
                xPos += 1;
                yPos += 1;
                box.style.right = `${screenWidth - xPos}px`;
                box.style.bottom = `${screenHeight - yPos}px`;
                setTimeout(moveBox, 500);
            }
        };

        moveBox();
    </script>

## Installation
- There was no need for any instalation, it was actually stright forward requires no installation and to be honest it was an awsome experience


## Usage
- After completing each of the given task what i do is test it with the help of gandalf to see if the code is actually working properly before pushing into my repository.

./The next thing is submitting it after pushing and making sure that everything is perfect, and moving to hte next quest and other activities given for the day.


### The Core Team


<span><i>Made at <a href='https://qwasar.io'>Qwasar SV -- Software Engineering School</a></i></span>
<span><img alt='Qwasar SV -- Software Engineering School's Logo' src='https://storage.googleapis.com/qwasar-public/qwasar-logo_50x50.png' width='20px' /></span>
