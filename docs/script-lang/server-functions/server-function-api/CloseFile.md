---
layout: default
title: OpenFile
nav_exclude: true
---
<a href="javascript:history.back()">Go Back</a>
{: .btn }

## CloseFile
{: .fs-9 .fw-600 }


Description: This command opens the designated file and prepares it to be updated. The file must exists since this function will not create a new file.
{: .fs-4 .fw-300 .text-green-100 }

```cs
CloseFile(stream)
```

## Provided Function Parameters: 
{: .fs-4 .fw-600 }

| Function Parameter(s) | Parameter Order | DataType | Example/Expected Value | Is Required? |
|:-------------|:------------------|:------------------|
| `stream` | 0 | Interger | `1326418` | Yes |

## Example Funtion Return Value:
{: .fs-4 .fw-600 }

| Return Value | DataType |
|:-------------|:------------------|
| `0` | Interger |

## Example Usage:
{: .fs-4 .fw-600 }

```cs
// Saves the filestream when a opening file.
filestream = OpenFile("somefolder\mytextfile.txt")

// Close the file that referenced in filestream.
CloseFile(filestream)
```