# son-devv
import 'package:flutter/material.dart';

void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  // This widget is the root of your application.
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      // Application name
      title: 'Flutter Stateful Clicker Counter',
      theme: ThemeData(
       
        primarySwatch: Colors.red,
      ),
      home: MyHomePage(title: 'Burak ana sayfasi'),
    );
  }
}

class MyHomePage extends StatefulWidget {
  final String title;
  const MyHomePage({Key? key, required this.title}) : super(key: key);

  te. Fields in a Widget subclass are
  
  @override
  _MyHomePageState createState() => _MyHomePageState();
}

class _MyHomePageState extends State<MyHomePage> {
  int _counter = 0;

  void _incrementCounter() {
    setState(() {
      
      _counter++;
    });
  }

  @override
  Widget build(BuildContext context) {
    
    return Scaffold(
      appBar: AppBar(
        
        title: Text(widget.title),
      ),
      body: Center(
        
        child: Column(
          
          mainAxisAlignment: MainAxisAlignment.center,
          children: <Widget>[
            Text(
              'kac kere bastıgını gosterir:',
            ),
            Text(
              '$_counter',
              style: TextStyle(fontSize: 25),
            ),
          ],
        ),
      ),
      floatingActionButton: FloatingActionButton(
        onPressed: _incrementCounter,
        tooltip: 'Increment',
        child: Icon(Icons.add),
      ), // This trailing comma makes auto-formatting nicer for build methods.
    );
  }
}
Form(
  child: Column(
    children: [
      FormField(
        builder: (FormFieldState state) {
          return Autocomplete(
            suggestions: names,
            onChanged: (String value) {
              state.didChange(value);
            },
            decoration: InputDecoration(
              labelText: 'Ad',
              suffixIcon: RawKeyboardListener(
                focusNode: _firstNameFocus,
                onKey: (RawKeyEvent event) {
                  if (event is RawKeyDownEvent) {
                    // Klavye girdisi alındığında önerileri filtreleyin
                  }
                },
              ),
            ),
          );
        },
      ),
      FormField(
        builder: (FormFieldState state) {
          return Autocomplete(
            suggestions: names,
            onChanged: (String value) {
              state.didChange(value);
            },
            decoration: InputDecoration(
              labelText: 'Soyad',
              suffixIcon: RawKeyboardListener(
                focusNode: _lastNameFocus,
                onKey: (RawKeyEvent event) {
                  if (event is RawKeyDownEvent) {
                    // Klavye girdisi alındığında önerileri filtreleyin
                  }
                },
              ),
            ),
          );
        },
      ),
    ],
  ),
)
Container(
  width: 200,
  height: 200,
  color: Colors.red,
  child: Center(
    child: Text('İbrahım hocam nasılsınız'),
  ),
),

FractionallySizedBox(
  widthFactor: 0.5,
  child: Image.asset('https://pbs.twimg.com/profile_images/1343911104053972998/HQdPfcaj_400x400.jpg'),
),

Padding(
  padding: EdgeInsets.only(top: 20),
  child: Image.asset('https://pbs.twimg.com/profile_images/1343911104053972998/HQdPfcaj_400x400.jpg'),
),
Transform(
  transform: Matrix4.diagonal3Values(1.0, 0.5, 1.0)..rotateZ(pi / 2),
  child: Image.asset('https://pbs.twimg.com/profile_images/1343911104053972998/HQdPfcaj_400x400.jpg'),
),
