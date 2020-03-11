# React Native Motion List
Change your application from the left one to the right one! Animate it!  **Easily!** [Animated Transition Article](http://bit.ly/animated-transition) or [Animated Graph Article](http://bit.ly/animated-graph)

<img src="https://github.com/xotahal/ui-interactions-detail-view/blob/master/assets/Final%20-%20Without%20animation.gif" width="240"><img src="https://github.com/xotahal/ui-interactions-detail-view/blob/master/assets/Final.gif" width="240">

### Getting Started
```bash
$ yarn add react-native-advance-motion-list
```

### Usage of SharedElement
We need to specify source and destination for shared element. This library then will move the shared element from source position to destination position.

```js
class Main extends Component {
  render() {
    return (
      <SharedElementRenderer>
        <App />
      </SharedElementRenderer>
    );
  }
}
```
```js
// List items page with source of SharedElement
import { SharedElement } from 'react-native-advance-motion-list';

class ListPage extends Component {
  render() {
    return (
      <SharedElement id="source">
        <View>{listItemNode}</View>
      </SharedElement>
    );
  }
}
```
```js
// Detail page with a destination shared element
import { SharedElement } from 'react-native-advance-motion-list';

class DetailPage extends Component {
  render() {
    return (
      <SharedElement sourceId="source">
        <View>{listItemNode}</View>
      </SharedElement>
    );
  }
}
```

## Author
- Mr-Strike
