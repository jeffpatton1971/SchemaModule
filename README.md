[![GitHub issues](https://img.shields.io/github/issues/SchemaModule/PowerShell)](https://github.com/SchemaModule/PowerShell/issues)
[![GitHub forks](https://img.shields.io/github/forks/SchemaModule/PowerShell)](https://github.com/SchemaModule/PowerShell/network)
[![GitHub license](https://img.shields.io/github/license/SchemaModule/PowerShell)](https://github.com/SchemaModule/PowerShell/blob/master/LICENSE)

## [ConvertFrom-SchemaArray](docs/ConvertFrom-SchemaArray.md)

```

NAME
    ConvertFrom-SchemaArray

SYNOPSIS
    This function takes the schemaArray object and converts it into a PowerShell array that can be nicely output as a JSON string.


SYNTAX
    ConvertFrom-SchemaArray [-Array] <System.Object> [[-Depth] <System.Int32>] [<CommonParameters>]


DESCRIPTION
    This function takes the schemaArray object and converts it into a PowerShell array that can be nicely output as a JSON string. This function is useful when you need to output the JSON schema as a JSON object. This would have the
    effect of creating an empty JSON document based on the schema that was provided.


RELATED LINKS
    Online Version: https://github.com/SchemaModule/PowerShell/blob/master/docs/ConvertFrom-SchemaArray.md#convertfrom-schemaarray
    ConvertFrom-SchemaObject https://github.com/SchemaModule/PowerShell/blob/master/docs/ConvertFrom-SchemaObject.md#convertfrom-schemaobject
    About Classes https://github.com/SchemaModule/PowerShell/blob/master/docs/about_Schema_Classes.md
    JSON Schema Array https://json-schema.org/understanding-json-schema/reference/array.html

REMARKS
    To see the examples, type: "get-help ConvertFrom-SchemaArray -examples".
    For more information, type: "get-help ConvertFrom-SchemaArray -detailed".
    For technical information, type: "get-help ConvertFrom-SchemaArray -full".
    For online help, type: "get-help ConvertFrom-SchemaArray -online"
```

## [New-SchemaBoolean](docs/New-SchemaBoolean.md)

```

CommonParameters         : True
WorkflowCommonParameters : False
details                  : @{name=New-SchemaBoolean; noun=; verb=}
Syntax                   : @{syntaxItem=System.Object[]}
parameters               : @{parameter=System.Object[]}
inputTypes               : @{inputType=}
relatedLinks             : @{navigationLink=System.Management.Automation.PSObject[]}
returnValues             : @{returnValue=}
aliases                  : None

remarks                  : Get-Help cannot find the Help files for this cmdlet on this computer. It is displaying only partial help.
                               -- To download and install Help files for the module that includes this cmdlet, use Update-Help.
                               -- To view the Help topic for this cmdlet online, type: "Get-Help New-SchemaBoolean -Online" or
                                  go to https://github.com/SchemaModule/PowerShell/blob/master/docs/New-SchemaBoolean.md#new-schemaboolean.
alertSet                 :
description              :
examples                 :
Synopsis                 :
                           New-SchemaBoolean [-id <string>] [-ref <string>] [-title <string>] [-description <string>] [-default <bool>] [-WhatIf] [-Confirm] [<CommonParameters>]

ModuleName               : schema
nonTerminatingErrors     :
xmlns:command            : http://schemas.microsoft.com/maml/dev/command/2004/10
xmlns:dev                : http://schemas.microsoft.com/maml/dev/2004/10
xmlns:maml               : http://schemas.microsoft.com/maml/2004/10
Name                     : New-SchemaBoolean
Category                 : Function
Component                :
Role                     :
Functionality            :

```

## [Get-SchemaDefinition](docs/Get-SchemaDefinition.md)

```
NAME
    Get-SchemaDefinition

SYNOPSIS
    A function to follow the Definition keyword and return the referenced schema


SYNTAX
    Get-SchemaDefinition [[-Reference] <System.Uri>] [<CommonParameters>]


DESCRIPTION
    A function to follow the Definition keyword and return the referenced schema. This function is mostly used in conjunction with Get-SchemaReference when processing a larger schema that has been broken into multiple files.


RELATED LINKS
    Online Version: https://github.com/SchemaModule/PowerShell/blob/master/docs/Get-SchemaDefinition.md#get-schemadefinition
    Get-SchemaDocument https://github.com/SchemaModule/PowerShell/blob/master/docs/Get-SchemaDocument.md#get-schemadocument
    ConvertTo-SchemaElement https://github.com/SchemaModule/PowerShell/blob/master/docs/ConvertTo-SchemaElement.md#convertto-schemaelement
    About Classes https://github.com/SchemaModule/PowerShell/blob/master/docs/about_Schema_Classes.md
    JSON Schema Reference https://json-schema.org/understanding-json-schema/reference/index.html

REMARKS
    To see the examples, type: "get-help Get-SchemaDefinition -examples".
    For more information, type: "get-help Get-SchemaDefinition -detailed".
    For technical information, type: "get-help Get-SchemaDefinition -full".
    For online help, type: "get-help Get-SchemaDefinition -online"
```

## [Format-SchemaDocument](docs/Format-SchemaDocument.md)

```
NAME
    Format-SchemaDocument

SYNOPSIS
    A simple schema linter


SYNTAX
    Format-SchemaDocument [-json] <System.String> [<CommonParameters>]


DESCRIPTION
    A simple schema linter to output classes into a format that the schema definition would expect. Limitations of PowerShell prevent property names from starting with '$' so the linter updates values like
    id,schema,definitions,references to be pre-fixed with a '$'.


RELATED LINKS
    Online Version: https://github.com/SchemaModule/PowerShell/blob/master/docs/Format-SchemaDocument.md#format-schemadocument
    Get-SchemaDocument https://github.com/SchemaModule/PowerShell/blob/master/docs/Get-SchemaDocument.md#get-schemadocument
    ConvertTo-SchemaElement https://github.com/SchemaModule/PowerShell/blob/master/docs/ConvertTo-SchemaElement.md#convertto-schemaelement
    About Classes https://github.com/SchemaModule/PowerShell/blob/master/docs/about_Schema_Classes.md
    JSON Schema Reference https://json-schema.org/understanding-json-schema/reference/index.html

REMARKS
    To see the examples, type: "get-help Format-SchemaDocument -examples".
    For more information, type: "get-help Format-SchemaDocument -detailed".
    For technical information, type: "get-help Format-SchemaDocument -full".
    For online help, type: "get-help Format-SchemaDocument -online"
```

## [Get-SchemaDocument](docs/Get-SchemaDocument.md)

```
NAME
    Get-SchemaDocument

SYNOPSIS
    This function will return a schemaDocument object of the input Schema.


SYNTAX
    Get-SchemaDocument [[-Path] <System.String>] [<CommonParameters>]


DESCRIPTION
    This function will return a schemaDocument object of the input Schema. This will help in building PowerShell objects that can be defined by a JSON schema. This allows a script to dynamically build objects based on a well-defined
    JSON schema.


RELATED LINKS
    Online Version: https://github.com/SchemaModule/PowerShell/blob/master/docs/Get-SchemaDocument.md#get-schemadocument
    ConvertTo-SchemaElement https://github.com/SchemaModule/PowerShell/blob/master/docs/ConvertTo-SchemaElement.md#convertto-schemaelement
    About Classes https://github.com/SchemaModule/PowerShell/blob/master/docs/about_Schema_Classes.md
    Schema Keyword https://json-schema.org/understanding-json-schema/reference/schema.html

REMARKS
    To see the examples, type: "get-help Get-SchemaDocument -examples".
    For more information, type: "get-help Get-SchemaDocument -detailed".
    For technical information, type: "get-help Get-SchemaDocument -full".
    For online help, type: "get-help Get-SchemaDocument -online"
```

## [ConvertTo-SchemaElement](docs/ConvertTo-SchemaElement.md)

```
NAME
    ConvertTo-SchemaElement

SYNOPSIS
    This function takes the output of ConvertFrom-Json CmdLet and converts it into SchemaModule classes.


SYNTAX
    ConvertTo-SchemaElement [-Object] <System.Object> [<CommonParameters>]


DESCRIPTION
    This function takes the output of ConvertFrom-Json CmdLet and converts it into SchemaModule classes. The input to ConvertFrom-Json should be a proper JSON schema file, or a file with proper JSON schema objects. It will then convert
    those into one of the defined classes schemaDocument, schemaObject, schemaArray, schemaString, schemaInteger, schemaNumber or schemaBoolean.


RELATED LINKS
    Online Version: https://github.com/SchemaModule/PowerShell/blob/master/docs/ConvertTo-SchemaElement.md#convertto-schemaelement
    Get-SchemaDocument https://github.com/SchemaModule/PowerShell/blob/master/docs/Get-SchemaDocument.md#get-schemadocument
    New-SchemaProperty https://github.com/SchemaModule/PowerShell/blob/master/docs/New-SchemaProperty.md#new-schemaproperty
    About Classes https://github.com/SchemaModule/PowerShell/blob/master/docs/about_Schema_Classes.md
    JSON Schema Reference https://json-schema.org/understanding-json-schema/reference/index.html

REMARKS
    To see the examples, type: "get-help ConvertTo-SchemaElement -examples".
    For more information, type: "get-help ConvertTo-SchemaElement -detailed".
    For technical information, type: "get-help ConvertTo-SchemaElement -full".
    For online help, type: "get-help ConvertTo-SchemaElement -online"
```

## [Find-SchemaElement](docs/Find-SchemaElement.md)

```
NAME
    Find-SchemaElement

SYNOPSIS
    This function provides the ability to find objects within the JSON schema either by Name, by Type or by a Path.


SYNTAX
    Find-SchemaElement [-ElementName <System.String>] -Schema <System.Object> [<CommonParameters>]

    Find-SchemaElement [-ElementPath <System.String>] -Schema <System.Object> [<CommonParameters>]

    Find-SchemaElement [-ElementType {schemaString | schemaNumber | schemaInteger | schemaObject | schemaBoolean | schemaArray | schemaDocument}] -Schema <System.Object> [<CommonParameters>]


DESCRIPTION
    This function provides the ability to find objects within the JSON schema either by Name, by Type or by a Path. A search by Name allows you to simply enter the name of the item you are looking for regardless of the underlying
    object type. This could potentially return any object that matches the Name provided. A search by Type allows you to find types within an object, this will likely always return multiple results.

    A search by Path is a little different as there is no real path per se. I borrowed a little bit from XPath and later iterations may borrow more heavily from there as it seems to make some sense. XPath
    (https://en.wikipedia.org/wiki/XPath)Basically we create a path based on where we are using a '/' to progress through objects and arrays in a fashion similar to navigating a path in a filesystem. It can be more easily seen when a
    JSON schema is rendered as text. For example if we wanted to view the Computer object within our Room schema it would look like this.

    $Schema.properties.contents.items.anyOf.properties.computers

    Whereas using a simple path notation it could more easily be viewed like this.

    $jPath = '/contents/computers'


RELATED LINKS
    Online Version: https://github.com/SchemaModule/PowerShell/blob/master/docs/Find-SchemaElement.md#find-schemaelement
    About Classes https://github.com/SchemaModule/PowerShell/blob/master/docs/about_Schema_Classes.md
    JSON Schema Reference https://json-schema.org/understanding-json-schema/reference/index.html

REMARKS
    To see the examples, type: "get-help Find-SchemaElement -examples".
    For more information, type: "get-help Find-SchemaElement -detailed".
    For technical information, type: "get-help Find-SchemaElement -full".
    For online help, type: "get-help Find-SchemaElement -online"
```

## [New-SchemaElement](docs/New-SchemaElement.md)

```
NAME
    New-SchemaElement

SYNOPSIS
    A function to create new SchemaModule objects


SYNTAX
    New-SchemaElement [[-Type] {string | number | integer | object | boolean | array | document}] [<CommonParameters>]


DESCRIPTION
    A function to create new SchemaModule objects


RELATED LINKS
    Online Version: https://github.com/SchemaModule/PowerShell/blob/master/docs/New-SchemaElement.md#new-schemaelement
    New-SchemaString https://github.com/SchemaModule/PowerShell/blob/master/docs/New-SchemaString.md#new-schemastring
    New-SchemaNumber https://github.com/SchemaModule/PowerShell/blob/master/docs/New-SchemaNumber.md#new-schemanumber
    New-SchemaInteger https://github.com/SchemaModule/PowerShell/blob/master/docs/New-SchemaInteger.md#new-schemainteger
    About Classes https://github.com/SchemaModule/PowerShell/blob/master/docs/about_Schema_Classes.md
    JSON Schema Reference https://json-schema.org/understanding-json-schema/reference/index.html

REMARKS
    To see the examples, type: "get-help New-SchemaElement -examples".
    For more information, type: "get-help New-SchemaElement -detailed".
    For technical information, type: "get-help New-SchemaElement -full".
    For online help, type: "get-help New-SchemaElement -online"
```

## [New-SchemaInteger](docs/New-SchemaInteger.md)

```
NAME
    New-SchemaInteger

SYNOPSIS
    A function to create new Schema Integer object


SYNTAX
    New-SchemaInteger [-default <System.Int32>] [-description <System.String>] [-enum <System.Int32[]>] [-examples <System.Int32[]>] [-exclusiveMaximum <System.Int32>] [-exclusiveMinimum <System.Int32>] [-id <System.String>] [-maximum
    <System.Int32>] [-minimum <System.Int32>] [-multipleOf <System.Int32>] [-ref <System.String>] [-title <System.String>] [<CommonParameters>]


DESCRIPTION
    A function to create new Schema Integer object


RELATED LINKS
    Online Version: https://github.com/SchemaModule/PowerShell/blob/master/docs/New-SchemaInteger.md#new-schemainteger
    New-SchemaElement https://github.com/SchemaModule/PowerShell/blob/master/docs/New-SchemaElement.md#new-schemaelement
    About Classes https://github.com/SchemaModule/PowerShell/blob/master/docs/about_Schema_Classes.md
    JSON Schema Reference https://json-schema.org/understanding-json-schema/reference/index.html

REMARKS
    To see the examples, type: "get-help New-SchemaInteger -examples".
    For more information, type: "get-help New-SchemaInteger -detailed".
    For technical information, type: "get-help New-SchemaInteger -full".
    For online help, type: "get-help New-SchemaInteger -online"
```

## [New-SchemaNumber](docs/New-SchemaNumber.md)

```
NAME
    New-SchemaNumber

SYNOPSIS
    A function to create new Schema Number object


SYNTAX
    New-SchemaNumber [-default <System.Decimal>] [-description <System.String>] [-examples <System.Decimal[]>] [-exclusiveMaximum <System.Decimal>] [-exclusiveMinimum <System.Decimal>] [-id <System.String>] [-maximum <System.Decimal>]
    [-minimum <System.Decimal>] [-multipleOf <System.Decimal>] [-ref <System.String>] [-title <System.String>] [<CommonParameters>]


DESCRIPTION
    A function to create new Schema Number object


RELATED LINKS
    Online Version: https://github.com/SchemaModule/PowerShell/blob/master/docs/New-SchemaNumber.md#new-schemanumber
    New-SchemaElement https://github.com/SchemaModule/PowerShell/blob/master/docs/New-SchemaElement.md#new-schemaelement
    About Classes https://github.com/SchemaModule/PowerShell/blob/master/docs/about_Schema_Classes.md
    JSON Schema Reference https://json-schema.org/understanding-json-schema/reference/index.html

REMARKS
    To see the examples, type: "get-help New-SchemaNumber -examples".
    For more information, type: "get-help New-SchemaNumber -detailed".
    For technical information, type: "get-help New-SchemaNumber -full".
    For online help, type: "get-help New-SchemaNumber -online"
```

## [ConvertFrom-SchemaObject](docs/ConvertFrom-SchemaObject.md)

```
NAME
    ConvertFrom-SchemaObject

SYNOPSIS
    This function takes the schemaObject object and converts it into a PowerShell object that can be nicely output as a JSON string.


SYNTAX
    ConvertFrom-SchemaObject [-Object] <System.Object> [[-Depth] <System.Int32>] [<CommonParameters>]


DESCRIPTION
    This function takes the schemaObject object and converts it into a PowerShell object that can be nicely output as a JSON string. This function is useful when you need to output the JSON schema as a JSON object. This would have the
    effect of creating an empty JSON document based on the schema that was provided.


RELATED LINKS
    Online Version: https://github.com/SchemaModule/PowerShell/blob/master/docs/ConvertFrom-SchemaObject.md#convertfrom-schemaobject
    ConvertFrom-SchemaArray https://github.com/SchemaModule/PowerShell/blob/master/docs/ConvertFrom-SchemaArray.md#convertfrom-schemaarray
    About Classes https://github.com/SchemaModule/PowerShell/blob/master/docs/about_Schema_Classes.md
    JSON Schema Object https://json-schema.org/understanding-json-schema/reference/object.html

REMARKS
    To see the examples, type: "get-help ConvertFrom-SchemaObject -examples".
    For more information, type: "get-help ConvertFrom-SchemaObject -detailed".
    For technical information, type: "get-help ConvertFrom-SchemaObject -full".
    For online help, type: "get-help ConvertFrom-SchemaObject -online"
```

## [New-SchemaProperty](docs/New-SchemaProperty.md)

```
NAME
    New-SchemaProperty

SYNOPSIS
    A Function to create either an object property or array item


SYNTAX
    New-SchemaProperty [[-Name] <System.String>] [[-Value] {schemaDocument | schemaNumber | schemaInteger | schemaString | schemaObject | schemaArray | schemaBoolean}] [[-Array] {allOf | anyOf | oneOf}] [<CommonParameters>]


DESCRIPTION
    A Function to create either an object property or array item.


RELATED LINKS
    Online Version: https://github.com/SchemaModule/PowerShell/blob/master/docs/New-SchemaProperty.md#new-schemaproperty
    ConvertTo-SchemaElement https://github.com/SchemaModule/PowerShell/blob/master/docs/ConvertTo-SchemaElement.md#convertto-schemaelement
    JSON Combining Schemas http://json-schema.org/understanding-json-schema/reference/combining.html#combining

REMARKS
    To see the examples, type: "get-help New-SchemaProperty -examples".
    For more information, type: "get-help New-SchemaProperty -detailed".
    For technical information, type: "get-help New-SchemaProperty -full".
    For online help, type: "get-help New-SchemaProperty -online"
```

## [Get-SchemaReference](docs/Get-SchemaReference.md)

```
NAME
    Get-SchemaReference

SYNOPSIS
    A function to follow the ref keyword and return the referenced schema


SYNTAX
    Get-SchemaReference [[-Reference] <System.Uri>] [<CommonParameters>]


DESCRIPTION
    A function to follow the ref keyword and return the referenced schema. This function is mostly used in conjunction with Get-SchemaDefinition and Get-SchemaDocument when processing a larger schema that has been broken into multiple
    files.


RELATED LINKS
    Online Version: https://github.com/SchemaModule/PowerShell/blob/master/docs/Get-SchemaReference.md#get-schemareference
    Get-SchemaDocument https://github.com/SchemaModule/PowerShell/blob/master/docs/Get-SchemaDocument.md#get-schemadocument
    ConvertTo-SchemaElement https://github.com/SchemaModule/PowerShell/blob/master/docs/ConvertTo-SchemaElement.md#convertto-schemaelement
    About Classes https://github.com/SchemaModule/PowerShell/blob/master/docs/about_Schema_Classes.md
    JSON Schema Reference https://json-schema.org/understanding-json-schema/reference/index.html

REMARKS
    To see the examples, type: "get-help Get-SchemaReference -examples".
    For more information, type: "get-help Get-SchemaReference -detailed".
    For technical information, type: "get-help Get-SchemaReference -full".
    For online help, type: "get-help Get-SchemaReference -online"
```

## [New-SchemaString](docs/New-SchemaString.md)

```
NAME
    New-SchemaString

SYNOPSIS
    A function to create new Schema String object


SYNTAX
    New-SchemaString [-default <System.String>] [-description <System.String>] [-enum <System.String[]>] [-examples <System.String[]>] [-id <System.String>] [-maxLength <System.Int32>] [-minLength <System.Int32>] [-pattern
    <System.String>] [-ref <System.String>] [-title <System.String>] [<CommonParameters>]


DESCRIPTION
    A function to create new Schema String object


RELATED LINKS
    Online Version: https://github.com/SchemaModule/PowerShell/blob/master/docs/New-SchemaString.md#new-schemastring
    New-SchemaElement https://github.com/SchemaModule/PowerShell/blob/master/docs/New-SchemaElement.md#new-schemaelement
    About Classes https://github.com/SchemaModule/PowerShell/blob/master/docs/about_Schema_Classes.md
    JSON Schema Reference https://json-schema.org/understanding-json-schema/reference/index.html

REMARKS
    To see the examples, type: "get-help New-SchemaString -examples".
    For more information, type: "get-help New-SchemaString -detailed".
    For technical information, type: "get-help New-SchemaString -full".
    For online help, type: "get-help New-SchemaString -online"
```
