new Vue({
el: '#app',
vuetify: new Vuetify(),
data: function() {
return {
myItems: ["Value1", "Value2"],
headers: [{
text: 'Column',
value: 'item' // Must match the key used in `myItemsTransformed`
}]
}
},
computed: {
myItemsTransformed() {
return this.myItems.map(item => ({ item }));
}
}
});
