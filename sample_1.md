import 'package:flutter/material.dart';

void main() {
  runApp(new MyApp());
}
class MyApp extends StatelessWidget {

  @override
  Widget build(BuildContext context) {
    return new MaterialApp(
      title: 'Generated App',
      theme: new ThemeData(
        primarySwatch: Colors.purple,
        primaryColor: const Color(0xFF9c27b0),
        accentColor: const Color(0xFF9c27b0),
        canvasColor: const Color(0xFF2499bc),
      ),
      home: new MyHomePage(),
    );
  }
}

class MyHomePage extends StatefulWidget {
  MyHomePage({Key key}) : super(key: key);
  @override
  _MyHomePageState createState() => new _MyHomePageState();
}

class _MyHomePageState extends State<MyHomePage> {
    @override
    Widget build(BuildContext context) {
      return new Scaffold(
        bottomNavigationBar: new BottomNavigationBar(
          items: [
            new BottomNavigationBarItem(
              icon: const Icon(Icons.visibility),
              title: new Text('Title'),
            ),
    
            new BottomNavigationBarItem(
              icon: const Icon(Icons.skip_next),
              title: new Text('Title'),
            ),
    
            new BottomNavigationBarItem(
              icon: const Icon(Icons.sim_card_alert),
              title: new Text('Title'),
            ),
    
            new BottomNavigationBarItem(
              icon: const Icon(Icons.star),
              title: new Text('Title'),
            ),
    
            new BottomNavigationBarItem(
              icon: const Icon(Icons.signal_wifi_4_bar),
              title: new Text('Title'),
            )
          ]
    
        ),
      );
    }
}
