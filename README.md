<h1 align="center"> 
C# Extension Methods
</h1>
<h2 align="center">
Minimal Pack
</h2>
#My C# Extension methods for collections and POCO objects. Enjoy! :collision:

## [ NUGET ](https://www.nuget.org/packages/Pylypeiev.Extensions.MinimalPack)  :hammer: 
[![NuGet version](https://badge.fury.io/nu/Pylypeiev.Extensions.MinimalPack.svg)](https://badge.fury.io/nu/Pylypeiev.Extensions.MinimalPack)

## [ Full Pack ](https://github.com/pylypeiev/CSharpExtensionMethods)  :eyes: 
[![NuGet version](https://badge.fury.io/nu/Pylypeiev.Extensions.svg)](https://badge.fury.io/nu/Pylypeievs.Extension)

## Table of Contents:
#### Collections extension methods
- [Array](#array)
- [Dictionary](#dictionary)
- [ICollection](#icollection)
- [IEnumerable](#ienumerable)
- [IList](#ilist)

#### POCO extension methods
- [ByteArray](#byte)
- [object](#object)
- [string](#string)
- [char](#char)
- [Exception](#exception)

## Collections extension methods
<a name="array"></a>

### Array extension methods:
- [Clear](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Collections%20extensions/ArrayExtensions.cs) - Sets a range of elements in an array to the default value of each element type.
- [Join](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Collections%20extensions/ArrayExtensions.cs) -  Concatenates the elements of an object array, using the specified separator between each element
- [ToArrayString](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Collections%20extensions/ArrayExtensions.cs) - A simple string representation of an array(regular, 2d, jagged)
<a name="dictionary"></a>

### Dictionary extension methods:
- [AddIfNotContainsKey](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Collections%20extensions/DictionaryExtensions.cs) - Add an element with provided key to dictionary if this key is not exist yet
- [AddOrUpdate](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Collections%20extensions/DictionaryExtensions.cs) - Add an element with provided key to dictionary, if this key is exist - update value
- [ToTuple](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Collections%20extensions/DictionaryExtensions.cs) - Convert this dictionary to list of Tuples, where item1 is key and item2 is a value from this dictionary
- [GetValueOrDefault](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Collections%20extensions/DictionaryExtensions.cs) - Get an element with provided key if this key is exist, otherwise default value

<a name="icollection"></a>

### ICollection extension methods:
- [AddIfNotContains](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Collections%20extensions/ICollectionExtensions.cs) - Add an element to the end of the collection if this value is not exist yet
- [AddRange](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Collections%20extensions/ICollectionExtensions.cs) - Adds the elements of the specified Array to the end of the collection
- [IsNullOrEmpty](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Collections%20extensions/ICollectionExtensions.cs) - Check if collection is null or empty 
- [RemoveRange](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Collections%20extensions/ICollectionExtensions.cs) - Removes a range of elements from collection


<a name="ienumerable"></a>

### IEnumerable extension methods:
- [Append](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Collections%20extensions/IEnumerableExtensions.cs) - Add the object top the end of IEnumerable
- [AreAllSame](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Collections%20extensions/IEnumerableExtensions.cs) - Check if all elements in IEnumerable are equals
- [Concatenate<string>](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Collections%20extensions/IEnumerableExtensions.cs) - Concatenates the elements of an IEnumerable<string> to 1 string
- [ForEach](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Collections%20extensions/IEnumerableExtensions.cs) - Performs the specified action on each element of the IEnumerable
- [IsEmpty](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Collections%20extensions/IEnumerableExtensions.cs) - Check if IEnumerable is empty
- [IsNotEmpty](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Collections%20extensions/IEnumerableExtensions.cs) - Check if IEnumerable is not empty 
- [IsNullOrEmpty](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Collections%20extensions/IEnumerableExtensions.cs) - Check if IEnumerable is null or empty
- [Join](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Collections%20extensions/IEnumerableExtensions.cs) - Concatenates the elements of an IEnumerable, using the specified separator between each element
- [Prepend](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Collections%20extensions/IEnumerableExtensions.cs) - Add the object at the beginning of IEnumerable
- [Shuffle](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Collections%20extensions/IEnumerableExtensions.cs) - Shuffle IEnumerable
- [PickRandom](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Collections%20extensions/IEnumerableExtensions.cs) - Pick N random elements from IEnumerable
- [ThisOrEmpty](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Collections%20extensions/IEnumerableExtensions.cs) - Safe foreach and more, returns an empty Enumerable if source is null
<a name="ilist"></a>

### IList extension methods:
 - [ChunkBy](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Collections%20extensions/IListExtensions.cs) - Chunk a list to smaller lists with a maximum capacity of the chunk size
 - [Clone](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Collections%20extensions/IListExtensions.cs) - Clone an collection to new IList
 - [Push](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Collections%20extensions/IListExtensions.cs) - Adds an object to the collection and return this collection for fluent api

## POCO extension methods:

<a name="byte"></a>

### ByteArray extension methods:
- [ToBase64String](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/ByteArray/ByteArrayExtensions.cs) - Converts an byte array to its equivalent string representation that is encoded with base-64.

### object extension methods:
- [IfNotNull](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/Object/ObjectGeneralExtensions.cs) - Perform action/function on the object if it not null 
- [IsIn](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/Object/ObjectGeneralExtensions.cs) - Determines if an object is contained in a sequence
- [IsNotNull](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/Object/ObjectGeneralExtensions.cs) - Check if object is NOT null
- [IsNull](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/Object/ObjectGeneralExtensions.cs) - Check if object is null
- [ToStringSafe](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/Object/ObjectGeneralExtensions.cs) - like ToString of the object, but not crushes if the object is null 
- [Try](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/Object/ObjectGeneralExtensions.cs) - Try to perform action/function on object
- [Yield](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/Object/ObjectGeneralExtensions.cs) - Wraps this object instance into an IEnumerable, consisting of a single item
- [DeepCopy](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/Object/ObjectGeneralExtensions.cs) - Deep copy of object using BinaryFormatter

<a name="string"></a>

### string extension methods:
- [ToDateTime](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/String/StringParsingExtensions.cs) - Convert to DateTime
- [ToDecimal](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/String/StringParsingExtensions.cs) - Convert to decimal
- [ToDouble](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/String/StringParsingExtensions.cs) - Convert to double
- [ToFloat](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/String/StringParsingExtensions.cs) - Convert to float
- [ToInt](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/String/StringParsingExtensions.cs) - Convert to int
- [ToLong](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/String/StringParsingExtensions.cs) - Convert to long
- [ToByteArray](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/String/StringParsingExtensions.cs) - Converts a string into an byte array
- [DecodeBase64](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/String/StringEncodingExtensions.cs) - Decodes a string encoded in base-64
- [EncodeBase64](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/String/StringEncodingExtensions.cs) - Encodes a string to its equivalent string representation that is encoded in base-64
- [RemoveFirst](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/String/StringOperationsExtensions.cs) - Remove the number of characters at the start of this string
- [RemoveFirstCharacter](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/String/StringOperationsExtensions.cs) - Remove the first character of this string
- [RemoveLast](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/String/StringOperationsExtensions.cs) - Remove the number of characters at the end of this string
- [RemoveLastCharacter](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/String/StringOperationsExtensions.cs) - Remove the last character of this string
- [Reverse](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/String/StringOperationsExtensions.cs) - Reverse the sequence of characters in this string
- [SurroundWith](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/String/StringOperationsExtensions.cs) - Surround this string with some string
- [TrimSafe](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/String/StringOperationsExtensions.cs) - Performs a trim only if the item is not null
- [ToLowerSafe](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/String/StringOperationsExtensions.cs) - Performs ToLower() only if input is not null
- [ToLowerInvariantSafe](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/String/StringOperationsExtensions.cs) - Performs ToLowerInvariant() only if input is not null
- [ToUpperSafe](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/String/StringOperationsExtensions.cs) - Performs ToUpper() only if input is not null
- [ToUpperInvariantSafe](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/String/StringOperationsExtensions.cs) - Performs ToUpperInvariant() only if input is not null
- [EndsWithIgnoreCase](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/String/StringSearchingExtensions.cs) - Determines whether the end of this string matches the specified string
- [EqualsIgnoreCase](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/String/StringSearchingExtensions.cs) - Determines whether two specified strings have the same value
- [IfNullThen](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/String/StringSearchingExtensions.cs) - Determines if the string is null or whitespace if yes returns nullAlternateValue
- [IsNullOrEmpty](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/String/StringSearchingExtensions.cs) - Indicates whether this string is null or an empty string
- [IsNullOrWhiteSpace](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/String/StringSearchingExtensions.cs) - Indicates whether this string is null, empty, or consists only of white-space characters 
- [NthIndexOf](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/String/StringSearchingExtensions.cs) - Reports the index of matched string regards to occurrenceNum
- [OccurrenceNum](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/String/StringSearchingExtensions.cs) - Reports the numbers of matches in this string
- [StartsWithIgnoreCase](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/String/StringSearchingExtensions.cs) - Determines whether the beginning of this string matches the specified string
- [ContainsInvariantSafe](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/String/StringSearchingExtensions.cs) - String.Contains with StringComparison parameter 

<a name="char"></a>

### char extension methods:
- [EqualsIgnoreCase](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/Char/CharExtensions.cs) - Determines whether two specified chars have the same value

<a name="exception"></a>

### Exception extension methods:
- [GetInnermostException](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/Exception/ExceptionExtensions.cs) - Get the innermost exception from this exception
- [GetInnerExceptions](https://github.com/pylypeiev/CSharpExtensionMethods/blob/master/Pylypeiev.Extensions/Objects%20Extensions/Exception/ExceptionExtensions.cs) - Get list of inner exceptions from this exception
