<p align="center"><img src="Controls.png"></p>
<h3>FXML for the above layout</h3>
<pre>
<GridPane fx:controller="sample.Controller"
          xmlns:fx="http://javafx.com/fxml" alignment="center" hgap="10" vgap="10">

    <Button GridPane.rowIndex="0" GridPane.columnIndex="0" text="Click Me">
        <graphic>
            <ImageView fitHeight="30" fitWidth="30">
                <Image url="@check.png"/>
            </ImageView>
        </graphic>
    </Button>

    <Label GridPane.rowIndex="0" GridPane.columnIndex="1" text="Label" textFill="blue">
        <font>
            <Font name="Comic Sans MS bold" size="20"/>
        </font>
        <graphic>
            <ImageView fitWidth="30" fitHeight="30">
                <Image url="@infoImage.png"/>
            </ImageView>
        </graphic>
    </Label>

    <fx:define>
        <ToggleGroup fx:id="colorToggleGroup"/>
    </fx:define>
    <VBox GridPane.rowIndex="0" GridPane.columnIndex="2" spacing="2">
        <Label text="Radio Button" textFill="white"
               style="-fx-label-padding:1;
                -fx-border-width:1;
                -fx-border-color:black;
                -fx-border-radius:10;
                -fx-background-color:black;
                -fx-background-radius:10"/>
        <RadioButton text="Red" toggleGroup="$colorToggleGroup"
                     selected="true"/>
        <RadioButton text="Blue" toggleGroup="$colorToggleGroup"/>
        <RadioButton text="Green" toggleGroup="$colorToggleGroup"/>
    </VBox>

    <VBox GridPane.rowIndex="0" GridPane.columnIndex="5" spacing="2">
        <Label text="Check Box" textFill="white"
               style="-fx-label-padding:1;
                -fx-border-width:1;
                -fx-border-color:black;
                -fx-border-radius:10;
                -fx-background-color:black;
                -fx-background-radius:10"/>
        <CheckBox text="Dog"/>
        <CheckBox text="Cat"/>
        <CheckBox text="Bird"/>
    </VBox>

    <VBox GridPane.rowIndex="0" GridPane.columnIndex="6" spacing="5" alignment="CENTER">
        <Label text="Toggle Button" textFill="white"
               style="-fx-label-padding:1;
                -fx-border-width:1;
                -fx-border-color:black;
                -fx-border-radius:10;
                -fx-background-color:black;
                -fx-background-radius:10"/>
        <HBox>
            <ToggleButton text="Toggle Me"/>
            <ToggleButton text="Hello"/>
            <ToggleButton text="Good-Bye"/>
        </HBox>

    </VBox>

    <VBox GridPane.rowIndex="1" GridPane.columnIndex="0" spacing="2">
        <Label text="Text Field" textFill="white"
               style="-fx-label-padding:1;
                -fx-border-width:1;
                -fx-border-color:black;
                -fx-border-radius:10;
                -fx-background-color:black;
                -fx-background-radius:10"/>
        <TextField/>
    </VBox>

    <VBox GridPane.rowIndex="1" GridPane.columnIndex="1" spacing="2">
        <Label text="Password Field" textFill="white"
               style="-fx-label-padding:1;
                -fx-border-width:1;
                -fx-border-color:black;
                -fx-border-radius:10;
                -fx-background-color:black;
                -fx-background-radius:10"/>
        <PasswordField/>
    </VBox>

    <VBox GridPane.rowIndex="1" GridPane.columnIndex="2" GridPane.columnSpan="3" alignment="CENTER" spacing="2">
        <Label text="ComboBox" textFill="white"
               style="-fx-label-padding:1;
                -fx-border-width:1;
                -fx-border-color:black;
                -fx-border-radius:10;
                -fx-background-color:black;
                -fx-background-radius:10"/>
        <ComboBox>
            <items>
                <FXCollections fx:factory="observableArrayList">
                    <String fx:value="Option 1"/>
                    <String fx:value="Option 2"/>
                    <String fx:value="Option 3"/>
                    <String fx:value="Option 4"/>
                    <String fx:value="Option 5"/>
                </FXCollections>
            </items>
            <value>
                <String fx:value="Select Option"/>
            </value>
        </ComboBox>

    </VBox>
    <VBox GridPane.rowIndex="1" GridPane.columnIndex="5" alignment="CENTER" spacing="2">
        <Label text="ChoiceBox" textFill="white"
               style="-fx-label-padding:1;
                -fx-border-width:1;
                -fx-border-color:black;
                -fx-border-radius:10;
                -fx-background-color:black;
                -fx-background-radius:10"/>
        <ChoiceBox prefWidth="120">
            <items>
                <FXCollections fx:factory="observableArrayList">
                    <String fx:value="Choice Box 1"/>
                    <String fx:value="Choice Box 2"/>
                    <String fx:value="Choice Box 3"/>
                    <String fx:value="Choice Box 4"/>
                    <String fx:value="Choice Box 5"/>
                </FXCollections>
            </items>
        </ChoiceBox>

    </VBox>
    <VBox GridPane.rowIndex="2" GridPane.columnIndex="0" GridPane.columnSpan="4" spacing="2">
        <Label text="Slider" textFill="white"
               style="-fx-label-padding:1;
                -fx-border-width:1;
                -fx-border-color:black;
                -fx-border-radius:10;
                -fx-background-color:black;
                -fx-background-radius:10"/>

        <Slider min="0" max="100"
                showTickLabels="true" showTickMarks="true" snapToTicks="true" minorTickCount="4"/>
    </VBox>

    <VBox GridPane.rowIndex="2" GridPane.columnIndex="4" spacing="2">
        <Label text="ChoiceBox" textFill="white"
               style="-fx-label-padding:1;
                -fx-border-width:1;
                -fx-border-color:black;
                -fx-border-radius:10;
                -fx-background-color:black;
                -fx-background-radius:10"/>
        <Spinner min="0" max="100" initialValue="50" editable="true"/>
    </VBox>

    <VBox GridPane.rowIndex="3" GridPane.columnIndex="0" spacing="2">
        <Label text="Color Picker" textFill="white"
               style="-fx-label-padding:1;
                -fx-border-width:1;
                -fx-border-color:black;
                -fx-border-radius:10;
                -fx-background-color:black;
                -fx-background-radius:10"/>
        <ColorPicker/>
    </VBox>

    <VBox GridPane.rowIndex="3" GridPane.columnIndex="1" spacing="2">
        <Label text="Date Picker" textFill="white"
               style="-fx-label-padding:1;
                -fx-border-width:1;
                -fx-border-color:black;
                -fx-border-radius:10;
                -fx-background-color:black;
                -fx-background-radius:10"/>
        <DatePicker/>
    </VBox>

    <VBox GridPane.rowIndex="3" GridPane.columnIndex="2" GridPane.columnSpan="3" spacing="2">
        <Label text="Titled Pane" textFill="white"
               style="-fx-label-padding:1;
                -fx-border-width:1;
                -fx-border-color:black;
                -fx-border-radius:10;
                -fx-background-color:black;
                -fx-background-radius:10"/>
        <Accordion expandedPane="$tp2">
            <panes>
                <TitledPane fx:id="tp1" text="Titled Pane 1">
                    <Label text="Label 1 in Titled Pane"/>
                </TitledPane>
                <TitledPane fx:id="tp2" text="Titled Pane 2">
                    <Label text="Label 2 in Titled Pane"/>
                </TitledPane>
                <TitledPane fx:id="tp3" text="Titled Pane 3">
                    <Label text="Label 3 in Titled Pane"/>
                </TitledPane>
            </panes>
        </Accordion>
    </VBox>


</GridPane>
</pre>
