# react-native-autoscroll-flatlist

An enhanced version of the original react-native `<FlatList>` component with built-in support for both Javascript and Typescript usage.

This component enables auto-scrolling on new item added to the list - which works like any chat client.

Note: only work for vertical orientation for now.

# Installation

`npm install --save react-native-autoscroll-flatlist`

or

`yarn add react-native-autoscroll-flatlist`

# Properties

This component extends the official [`FlatListProps`](https://facebook.github.io/react-native/docs/flatlist), with the only exclusion for `ref` prop.

# Example Usage

Import the component with:

```
import AutoScrollFlatList from "react-native-autoscroll-flatlist";
```

and simply use it like an ordinary `<FlatList>`, for example:

```
<AutoScrollFlatList
    data={myData}
    renderItem={({item, index}) => <YourComponent item={item} index={index} />}
    keyExtractor={item => item.id}
/>
```
