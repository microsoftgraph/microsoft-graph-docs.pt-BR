---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 68f2200f86a3cbf16241d984451133df71e97c82
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790350"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var index = new Int32
{
};

var values = JToken.Parse("[{}]");

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Columns
    .Add(index,values,null)
    .Request()
    .PostAsync();

```