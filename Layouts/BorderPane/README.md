<p align="center"><img src="BorderPane.png"></p>
<h3>FXML for the above layout</h3>
<pre>
&lt;BorderPane xmlns:fx="http://javafx.com/fxml"&gt;
    &lt;top&gt;
        &lt;Label text="This label is in the top position" alignment="CENTER"
               BorderPane.alignment="CENTER"/&gt;
    &lt;/top&gt;
    &lt;left&gt;
        &lt;Label text="This label is on the left"/&gt;
    &lt;/left&gt;
    &lt;center&gt;
        &lt;Label text="This is the center"/&gt;
    &lt;/center&gt;
    &lt;right&gt;
        &lt;Label text="This label is on the right"/&gt;
    &lt;/right&gt;
    &lt;bottom&gt;
        &lt;HBox spacing="10" alignment="CENTER"&gt;
            &lt;padding&gt;
                &lt;Insets left="10" bottom="10"/&gt;
            &lt;/padding&gt;
            &lt;Button text="Okay" prefWidth="90"/&gt;
            &lt;Button text="Cancel" prefWidth="90"/&gt;
            &lt;Button text="Help" prefWidth="90"/&gt;
        &lt;/HBox&gt;
    &lt;/bottom&gt;
&lt;/BorderPane&gt;
</pre>
