/_ Properties for other selectors _/

- {
  padding: 0;
  margin: 0;
  color: pink;
  }

.container {
min-height: 100vh;
background-color:bisque;
}

.letters {
display: flex;
justify-content: center;
padding-top: 20px;
margin-bottom: 20px;
text-transform:uppercase;
font-size: 60px;
}

/_ Add rules for the element 'p' present inside the class 'letters' using descendant selector _/
.letters p{
text-align: center;
background-color: rgb(250, 150, 100);
width: 70px;
margin-right: 2.5px;
border-radius: 15%;
border-color: rgb(250, 125, 75);
border-style: solid;

}

/_ Add rules for steps 8 and 9 _/
.letters:hover > p:nth-child(even) {
transform: rotateY(360deg) skew(10deg);
transition: 0.5s;
}

/_ Add rules for steps 10 and 11 _/
.letters:hover p:nth-child(odd) {
transform: rotateX(360deg) skew(10deg);
transition: 1.5s;
}
