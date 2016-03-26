# PyIEnumObjects

## PyIEnumObjects Object

Iterates through a number of arbitrary interfaces

#### Methods


  - [Next](PyIEnumObjects.md#pyienumobjectsnext)

    Retrieves a specified number of items in the enumeration sequence.&nbsp;

  - [Skip](PyIEnumObjects.md#pyienumobjectsskip)

    Skips over the next specified elementes.&nbsp;

  - [Reset](PyIEnumObjects.md#pyienumobjectsreset)

    Resets the enumeration sequence to the beginning.&nbsp;

  - [Clone](PyIEnumObjects.md#pyienumobjectsclone)

    Creates another enumerator that contains the same enumeration state as the current one.&nbsp;

## [PyIEnumObjects](#pyienumobjects).Clone

[PyIEnumObjects](#pyienumobjects)= __Clone(__ )
Creates another enumerator that contains the same enumeration state as the current one

## [PyIEnumObjects](#pyienumobjects).Next

([PyIUnknown](#pyiunknown),...) = __Next( *num*  *, riid* __ )
Retrieves a specified number of items in the enumeration sequence.

#### Parameters


  -  *num=1* : int

    Number of items to retrieve.

  -  *riid=IID_IUnknown* :[PyIID](#pyiid)

    The interfaces to return

## [PyIEnumObjects](#pyienumobjects).Reset

 __Reset(__ )
Resets the enumeration sequence to the beginning.

## [PyIEnumObjects](#pyienumobjects).Skip

 __Skip(__ )
Skips over the next specified elementes.