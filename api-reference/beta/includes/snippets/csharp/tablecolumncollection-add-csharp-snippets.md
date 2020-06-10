---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 11bc516ecd400cbc288c0f0b7734a64309379f22
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684004"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var index = new Int32
{
};

var values = JToken.Parse("[{}]");

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Columns
    .Add(index,values,null)
    .Request()
    .PostAsync();

```