- npm goes and installs express for u
- express is a package to use for json
- json is a data format
- cors is like middleware that wont allow u to access certain routes thru certain ips. like why would google allow me to access their admins page?
- middleware is like middle man that sits in between 
```
import { StatusBar } from 'expo-status-bar';
import { StyleSheet, Text, View, Button } from 'react-native';
import { TextInput } from 'react-native';
import { useState } from 'react';
export default function App() {

 const[test,settest]=useState("enter anything you want :)");
 //settest("barbie")
  return (
    <View style={styles.container}>
      <Text>avantika made this app! enjoy loves!</Text>
      <Text>{test}</Text>
      <StatusBar style="auto" />
      <TextInput style={styles.input}></TextInput>
      <Button title='the classic : do not press' onPress={()=>{settest("lmao, nothing happens when you press the button")}}></Button>

    </View>
  );
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
    backgroundColor: '#ff4777',
    alignItems: 'center',
    justifyContent: 'center',
  },
  test:{
    fontSize:20,
    margin:20
  },
  input:{
    borderWidth:1,
    borderColor:'white',
    padding:10,
    margin:15,
    width:200

  }
  }
);
```
