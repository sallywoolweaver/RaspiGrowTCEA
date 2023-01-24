# RaspiGrowTCEA

For use with https://learn.pimoroni.com/article/assembling-grow 

## After following the above instructions, if you want to edit the alarm software:
   In the terminal run: 
   - **sudo systemctl stop grow-monitor.service**
   - **sudo chmod a+w /usr/bin/grow-monitor**
     - This will stop the services then let you edit the files. Once you've finished your edits (make sure you are editing the usr/bin/grow-monitor file), start the service with
        - **sudo systemctl start grow-monitor.service**
      - Note - if you want to use the text messaging you need to use sudo pip install *packagename* in order to work
 
## If you want to edit the pump time or alarm time manually
-   In the terminal run: 
  - **sudo systemctl stop grow-monitor.service**
   - **sudo chmod a+w /etc/default/grow**
   - then edit the above file. When finished, re-start the service again
