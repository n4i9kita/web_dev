1. [Question 1](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/record-collection)
```js
// my solution
function updateRecords(records, id, prop, value) {
  if( value!="" && prop!='tracks')   records.id.prop=value;
  else if (prop=='tracks'){
    if(records[id].hasOwnProperty("tracks") === false) {records.id.prop=[value];}
    else if(value!="") records.id.tracks.push(value);
  }
  else if(value=="") delete records.id.prop;
  return records;
}

// TypeError: Cannot set properties of undefined (setting 'prop')
```
