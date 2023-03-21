# java-analog-clock

This is a Java program that displays an analog clock. The clock face is drawn using the drawOval() method of the Graphics class, and the clock hands are drawn using the drawLine() method.

The clock implements the Runnable interface, which allows it to run in a separate thread. The thread sleeps for 100 milliseconds and then calls the repaint() method, which causes the paint() method to be called again.

The clock is created using a JFrame and a JPanel. The JPanel is added to the JFrame, and the background color of the JFrame is set to a custom color.

The clock hands are drawn using the current time obtained from a Date object. The current second, minute, and hour are obtained using a SimpleDateFormat object, and then converted to the x and y coordinates for the clock hands using trigonometry.

The program uses a double-buffering technique to eliminate flicker. This is accomplished by overriding the update() method to call the paint() method, which draws the clock hands.

