---
title: "pair::second (STL/CLR) | Microsoft Docs"
ms.custom: ""
ms.date: "11/04/2016"
ms.technology: ["cpp-cli"]
ms.topic: "reference"
f1_keywords: ["cliext::pair::second"]
dev_langs: ["C++"]
helpviewer_keywords: ["second member [STL/CLR]"]
ms.assetid: f30d3d1f-c7be-45d2-92ff-6861b96a92ff
author: "mikeblome"
ms.author: "mblome"
ms.workload: ["cplusplus", "dotnet"]
---
# pair::second (STL/CLR)
The second wrapped value.  
  
## Syntax  
  
```  
Value2 second;  
```  
  
## Remarks  
 The object stores the second wrapped value.  
  
## Example  
  
```  
// cliext_pair_second.cpp   
// compile with: /clr   
#include <cliext/utility>   
  
int main()   
    {   
    cliext::pair<wchar_t, int> c1(L'x', 3);   
    System::Console::WriteLine("[{0}, {1}]", c1.first, c1.second);   
  
    cliext::pair<wchar_t, int>::first_type first_val = c1.first;   
    cliext::pair<wchar_t, int>::second_type second_val = c1.second;   
    System::Console::WriteLine("[{0}, {1}]", first_val, second_val);   
    return (0);   
    }  
  
```  
  
```Output  
[x, 3]  
```  
  
## Requirements  
 **Header:** \<cliext/utility>  
  
 **Namespace:** cliext  
  
## See Also  
 [pair (STL/CLR)](../dotnet/pair-stl-clr.md)   
 [pair::first (STL/CLR)](../dotnet/pair-first-stl-clr.md)   
 [pair::first_type (STL/CLR)](../dotnet/pair-first-type-stl-clr.md)   
 [pair::second_type (STL/CLR)](../dotnet/pair-second-type-stl-clr.md)