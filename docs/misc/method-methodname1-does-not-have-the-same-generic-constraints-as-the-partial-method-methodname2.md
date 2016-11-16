---
title: "Method &#39;&lt;methodname1&gt;&#39; does not have the same generic constraints as the partial method &#39;&lt;methodname2&gt;&#39; | Microsoft Docs"
ms.custom: ""
ms.date: "2015-07-20"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "devlang-visual-basic"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "bc31438"
  - "vbc31438"
helpviewer_keywords: 
  - "BC31438"
ms.assetid: ea092f0c-661b-49db-80c1-76401fc8bc0b
caps.latest.revision: 8
author: "stevehoag"
ms.author: "shoag"
manager: "wpickett"
translation.priority.ht: 
  - "de-de"
  - "es-es"
  - "fr-fr"
  - "it-it"
  - "ja-jp"
  - "ko-kr"
  - "ru-ru"
  - "zh-cn"
  - "zh-tw"
translation.priority.mt: 
  - "cs-cz"
  - "pl-pl"
  - "pt-br"
  - "tr-tr"
---
# Method &#39;&lt;methodname1&gt;&#39; does not have the same generic constraints as the partial method &#39;&lt;methodname2&gt;&#39;
You have defined a partial method implementation that has generic constraints that differ from the constraints in the partial method declaration. The following code illustrates the error.  
  
```vb#  
Partial Class Class1  
  
    Partial Private Sub Test(Of T As Class)(ByVal arg As T)  
    End Sub  
  
End Class  
  
Partial Class Class1  
  
    '' The error occurs here, for Test.  
    'Private Sub Test(Of T As Structure)(ByVal arg As T)  
    'End Sub  
  
End Class  
```  
  
 **Error ID:** BC31438  
  
## See Also  
 [Partial Methods](/dotnet/visual-basic/language-reference/procedures/partial-methods)   
 [Partial](/dotnet/visual-basic/language-reference/modifiers/partial)   
 [Generic Procedures in Visual Basic](/dotnet/visual-basic/programming-guide/language-features/data-types/generic-procedures)