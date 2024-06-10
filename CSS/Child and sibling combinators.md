


```bash
index.html

<body>



 <!--
-------------------------- This is a comment --------------------
    combinators = explain the relationship 
                  between listed selectors
                        = descendant
                    >   = child
                    ~   = general sibling 
                    +   = adjacent sibling
-------------------------- This is a comment --------------------
 -->


    <div id="container">
        <p>This is child1</p>
        <p>This is a child2</p>
            <div>
                <p>This is a grand-child</p>
            </div>
    </div>

    <p>This is general sibling1</p>
    <p>This is general sibling2</p>
    <p>This is general sibling3</p>
</body>

```

## Experiment any css child
- For example using this kind of example 

```bash
style.css


#container {
  border: 2px solid;
}

#container ~ p {
  background-color: yellow;
}
```
