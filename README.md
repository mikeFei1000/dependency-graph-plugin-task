# dependency-graph-plugin-task
Visual implementation of Module dependencies
## Usage
1. Copy ```projectDependencyGraph.gradle``` file to the root directory of the project
2. Add plugin to ```build.gradle``` in your app
```
apply from: "${project.rootProject.file('projectDependencyGraph.gradle')}"
```
3. run
```
./gradlew projectDependencyGraph
```
4. Project module dependency graph created at 
```build/reports/dependency-graph/project.dot```

* prview with markdown：

Copy the contents of ```project.dot``` to the online tool preview https://mermaid-js.github.io/mermaid-live-editor/
![mermaid-diagram-20220426112122](https://user-images.githubusercontent.com/20104311/165213800-f9b4c0fa-c8d7-41ee-b126-3bf5f192e946.png)

* prview with graphviz:

Using graphviz to generate local beautiful diagram, if not installed the local environment, Copy the contents of ```project_digraph.dot``` to the online tool preview
http://dreampuf.github.io/GraphvizOnline/

![graphviz](https://user-images.githubusercontent.com/20104311/165214479-affd0c81-032a-40ac-b1d4-4c28460b35dc.png)




