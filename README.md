BinaryTreeVisualizer
====================
**BinaryTreeVisualizer** consists of a Java implementation to create **Binary Search Trees** and some Javascript code to render these trees in a web page. I used this API
in my final year project (jSCAPE) to provide a visual aid to help students answer exercises on binary search trees.

###Files
The Java implementation resides in a single file called `BST.java`.
```java
    BST<Integer> bst = new BST();
    
    bst.insert(new Integer(34));
    bst.insert(new Integer(22));
    bst.insert(new Integer(28));
    bst.insert(new Integer(56));
    
    String bstJSON = bst.toJSON();
```
The code snippet above shows the creation of a binary tree, how to insert a few elements and how to get the JSON representation of the tree, so that it can be used by the visualizer. Take
a look at the rest of the API for other functions which can be called on binary search trees.

The Binary Search Tree visualizer is programmed in Javascript using the JIT library. The files for the visualizer are:

    -binary_tree.js
    
    -binary_tree.html
    
    -jit.js
    
    -Spacetree.css and base.css are modified versions of the original CSS files used for the Spacetree demo.
     Links to the originals: 
     http://philogb.github.io/jit/static/v20/Jit/Examples/css/base.css
     http://philogb.github.io/jit/static/v20/Jit/Examples/css/Spacetree.css
     
   
###TODO list   
* Write small tutorial on how to use the visualizer.
* Clean BST.java code and add documentation/comments...no need to use getters/setters for BSTNode, code is ugly.
* Explain JSON format for binary tree + example.
* Better layout for json string produced by toJSON().
* Clean up javascript code, html code.
* Add links to library and references used for this project.
* Comment on known bugs, i.e. sometimes if node has only one parent, it won't be at the correct location of its parent.
* Remove use of StringBuilder and just print the output out? or maybe two methods?
