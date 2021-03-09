﻿# zoom-clone

This solution is based on openvidu-call-react. The application license can be found here: http://www.apache.org/licenses/LICENSE-2.0

In order to be able to start the application in localhost, you need to have and openvidu server running. This can be done with this docker file:

docker run -p 4443:4443 --rm -e OPENVIDU_SECRET=MY_SECRET openvidu/openvidu-server-kms:2.16.0

this uses the port 4443 for the openvidu server (kurento media server) and MY_SECRET as password for the server. Username is OPENVIDUAPP. 

Then you need to open a separate terminal, navigate to openvidu-call-react/openvidu-call-react and execute

npm i

once the installations are done, execute

npm run

After this, the application can be opened in your browser under  http://localhost:3000 (Note: getUserMedia normally is allowed only on https, but as it is localhost, the browser should let the camera and microphone to be used). The first time you open it, it will report a certificate issue, you need to go to the "Advanced options" (in Chrome), and proceed to the page. You will be redirected to the server on port 4443: https://localhost:4443/accept-certificate if you see "accept-cert", you can open up the localhost:3000 again and the application should run now.

