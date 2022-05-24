# How to deploy an express.js file on netlify


1.Create a folder and initialize the folder

<img width="100" alt="Screenshot 2022-05-24 at 14 28 49" src="https://user-images.githubusercontent.com/74420607/170046776-178e68c3-8a7e-4c1f-9c87-2916fb0c062a.png">
<hr>
2.Install all the necessary dependencies 

<img width="286" alt="Screenshot 2022-05-24 at 14 29 42" src="https://user-images.githubusercontent.com/74420607/170046976-523f0d91-534b-4c8a-8e46-f90caa14e38a.png">
<hr>
netlify-lamda(serve our function locally and compile the functions for production)

serverless-http(take our express app and convert it in a lambda function)
<hr>
3.Create a git ignore file(ignore node modules and functions folder)

<img width="360" alt="Screenshot 2022-05-24 at 14 33 42" src="https://user-images.githubusercontent.com/74420607/170047823-07b1ee8a-b5c5-4929-ac0a-ca734458e16d.png">
<hr>
4.Set up netlify(netlify.toml file)
<img width="364" alt="Screenshot 2022-05-24 at 14 35 04" src="https://user-images.githubusercontent.com/74420607/170048114-a6eec69a-1585-4e7e-a8c5-d78aaf036801.png">
<hr>
5.We need to create a dist folder where we are going to create an empty index.html file(if we want to deploy something on netlify we need to have a dist folder on our app)

<img width="292" alt="Screenshot 2022-05-24 at 14 37 35" src="https://user-images.githubusercontent.com/74420607/170048694-7e331e35-2a7e-4ed7-97ed-dc699c5993e3.png">
<hr>
6.Create a src folder where we place our main js express file(api.js in this case)

-common js-
<img width="491" alt="Screenshot 2022-05-24 at 14 39 37" src="https://user-images.githubusercontent.com/74420607/170049194-1c122016-9786-407e-a2fc-b673fe6d718a.png">

-es module-
<img width="485" alt="Screenshot 2022-05-24 at 14 40 58" src="https://user-images.githubusercontent.com/74420607/170049516-b17628dd-e577-4d45-9bd6-a1485f8261fc.png">
<hr>
7. Create two script command on package.json to run lamda locally and on production

<img width="425" alt="Screenshot 2022-05-24 at 14 43 44" src="https://user-images.githubusercontent.com/74420607/170050237-6d8d0745-ebc9-4c45-a271-2621208215b1.png">

8.we run the app locally remeber to hit the URL specified on express(http://localhost:9000/.netlify/functions/api)




<img width="493" alt="Screenshot 2022-05-24 at 14 46 27" src="https://user-images.githubusercontent.com/74420607/170050939-bf55c4e2-f3b1-436d-89e7-abe99d245b11.png">







