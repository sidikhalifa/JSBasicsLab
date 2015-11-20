(function(global) {
    'use strict';

    var JS_BASICS={};

    JS_BASICS.isNumberEven = function(i) {
	return ( i % 2 === 0);
        // i will be an integer.
        // Return true if it's even, and false if it isn't.
    };

    JS_BASICS.getFileExtension = function(str) {
        // str will be a string, but it may not have a file extension.
// Return the file extension (with no period) if it has one, otherwise false
	 
		if (str.indexOf('.') !== -1){
			var  v= str.split('.') ;
	        	var r=v[v.length-1];
			return r;
		} else {
			return false;
		}

	    
	 };

    JS_BASICS.longestString = function(arr) {
        // arr will be an array.
        // Return the longest string in the array
	
	

	var x=arr;	
		var k=0;
	var l=x[k].length;
	if (typeof x[0] != 'string'){ l=1;}
	for(var i=1;i<x.length;i++) {
	var l1=x[i].length;
		if (typeof x[i] != 'string'){l1=1};
		if (l1>=l){
			k=i;
		}	
	}
	return x[k];


    };

    JS_BASICS.reverseString = function(str) {
        // str will be an string
        // Return a new string who's characters are in the opposite order to str's.
	//var x=new Array();
	/*var tab=str.split(".");
	var t=new Array(tab.length);
	for(var i=0;i<tab.length;i++){
		 t[i]=tab[i].reverse();
	}
	return t; */
	//var x=str.reverse();
	/*var x=str;
	
	if(typeof str === 'string'){
	       for (var i=x.length-1;i>-1;i--) x[x.length-1-i]=str[i];
	       return x; 
	}*/
	 return str.split("").reverse().join("");
	
    };

    JS_BASICS.isPalindrome = function(str) {
        // str will be an string
        // Return true if it is a palindrome and false otherwise. It should be case insensitive and not consider space or punctuation.

	var x1=str.split("").reverse().join("").replace(" ","").toLowerCase();
	var x2=str.split("").join("").replace(" ","").toLowerCase();
	
	/*	return true;
	       for (var i=0;i<x1.length;i++){ 
			if(x1[i]!=x2[x2.length-1 -i]){
				return false;
				
				
			}
		} */
			
	    return x1 == x2;
				
			 
	
	 
    };

    JS_BASICS.nestedSum = function(arr) {
        // arr will be an array, containing integers, strings and/or arrays like itself
        // Return the sum all the numbers you find, anywhere in the nest of arrays.
	
	var sum=0;
	for (var i=0;i<arr.length;i++){
		
		
		if(arr[i] instanceof Array){
			sum+=JS_BASICS.nestedSum(arr[i]);
		}
		if(arr[i] === Math.round(arr[i])){
			sum+=arr[i];
		}
		
	}	
	return sum;
		
	
    };

    global.JS_BASICS = JS_BASICS;
}(this));
