# SelectPresenter
React Native example app

### Description
This app is example built by react native. It just select someone on list of presenter or some purpose.    
React-Native is best choice if you need to develop on hybrid.

### App.js
```javascript
/**
 * SelectPresenter
 * https://github.com/facebook/react-native
 *
 * @author: Seonmeyong Kim <gumanhae@gmail.com>
 * @flow
 */

import React, {Component} from 'react';
import {Platform, StyleSheet, Text, View} from 'react-native';

const instructions = Platform.select({
  ios: 'Press Cmd+R to reload,\n' + 'Cmd+D or shake for dev menu',
  android:
    'Double tap R on your keyboard to reload,\n' +
    'Shake or press menu button for dev menu',
});

type Props = {};
export default class App extends Component<Props> {
  render() {
  			  	var arr = ["Person1", 
  					"Person2",
					"Person3",
					"Person4",
					"Person5",
					"Person6",
					"Person7",
					"Person8",
					"Person9",
					"Person10",
					"Person11",
					"Person12"];
			var a = arr[ Math.floor( Math.random() * arr.length ) ] ;
    return (
      <View style={styles.container}>
        <Text style={styles.welcome}>다음 iOS 스터디 발표자는 {a} 입니다!</Text>
      </View>
    );
  }
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
    justifyContent: 'center',
    alignItems: 'center',
    backgroundColor: '#F5FCFF',
  },
  welcome: {
    fontSize: 20,
    textAlign: 'center',
    margin: 10,
  },
  instructions: {
    textAlign: 'center',
    color: '#333333',
    marginBottom: 5,
  },
});

```
