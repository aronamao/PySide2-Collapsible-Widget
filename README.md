# PySide2 Collapsible Widget

Simple collapsible widget for PySide2, made to mimic Maya's native GUI


# How to use

Simply get the content widget via the contentWidget getter and attach your desired layout to it.

```python
layout = QtWidgets.QVBoxLayout()
container = Container("Group")
layout.addWidget(container)

content_layout = QtWidgets.QGridLayout(container.contentWidget)
content_layout.addWidget(QtWidgets.QPushButton("Button"))
```

This example is also available in the docstring of the Container class for easy access inside your IDE.

The Container class also has methods for collapsing, expanding and toggling the widget so you can hook them up to external buttons.

