<h4>1. Install Pixi on your machine</h4>

<p>Follow the installation guideline at: <a
    href="https://pixi.prefix.dev/latest/installation/">https://pixi.prefix.dev/latest/installation/</a><br>Pixi
  is a package management tool like conda, but <em>much</em> faster.</p>

<h4>2. Create Pixi workspace and environment for the course</h4>

<p>Navigate to whatever directory you want to use for the course. Place the <a
    href="../gds_py.yml">gds_py.yml</a>
  file there. Open a terminal window in that directory and execute 
  
```
pixi init  --import gds_py.yml
```
  
This sets up a Pixi workspace and environment in that directory, with all the dependencies that you need for the course.</p>

<h4>3. Install dependencies and start Jupyter Lab</h4>

<p>In the same terminal window, execute 

```
pixi run jupyter lab
```

The first time you do this, it may take several minutes, since Pixi has to install all the dependencies. After Pixi is finished, an instance of Jupyter lab is automatically going to open in your browser. </p> 

<p>Pixi will place a pixi.lock and a pixi.toml file in that folder. Keep those files, as they will allow you to restart the environment fast next time you need it, via <TT>pixi run jupyter lab</TT>.</p>

<p>If you prefer to use an IDE, rather than Jupyter Lab, please find documentation how to connect your IDE to the Pixi environmenthere: 

* VSCode: <a
    href="https://pixi.prefix.dev/latest/integration/editor/vscode/">https://pixi.prefix.dev/latest/integration/editor/vscode/</a>
* PyCharm: <a
    href="https://pixi.prefix.dev/latest/integration/editor/jetbrains/">https://pixi.prefix.dev/latest/integration/editor/jetbrains/</a>
</p>

<h4>4. Test requirements</h4>

<p>Try to run all of the <a
    href="./test_gdspy_install.ipynb">test_gdspy_install.ipynb</a>
  notebook. There could be a bunch of warnings thrown, for example in red cells,
  but as long as you arrive at the last cell without interruption you are good
  to go!</p>

<!---
<h4>5. Issues?</h4>
<p>We are sorry to hear. Our TA will use the first exercise to help with
  installations: Jan 28th from 12:20 in room 4A58. If you have any issues left
  <strong>after</strong> that session, please contact our TA to get it resolved.
</p>
--->