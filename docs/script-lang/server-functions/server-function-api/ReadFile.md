---
layout: default
title: ReadFile
nav_exclude: true
---
<a href="javascript:history.back()">Go Back</a>
{: .btn }

## ReadFile
{: .fs-9 .fw-600 }

Description: This command opens the designated file and prepares it to be updated. The file must exists since this function will not create a new file.
{: .fs-4 .fw-300 .text-green-100 }

```cs
ReadFile(filename)
```

## Provided Function Parameters: 
{: .fs-4 .fw-600 }

| Function Parameter(s) | Parameter Order | DataType | Example/Expected Value | Is Required? |
|:-------------|:------------------|:------------------|
| `filename` | 0 | String | `somefolder\mytextfile.txt` | Yes |

## Example Funtion Return Value:
{: .fs-4 .fw-600 }

| Return Value | DataType |
|:-------------|:------------------|
| `1326418` | Interger |

## Example Usage:
{: .fs-4 .fw-600 }

```cs
// Saves the filestream when a opening file.
filestream = ReadFile("somefolder\mytextfile.txt")
```