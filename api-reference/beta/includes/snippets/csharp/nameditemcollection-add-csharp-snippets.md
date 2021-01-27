---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d8d5ebb00bd0ad547e681af7c151eee538140869
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015109"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var name = "test5";

var reference = "=Sheet1!$F$15:$N$27";

var comment = "Comment for the named item";

await graphClient.Me.Drive.Items["{id}"].Workbook.Names
    .Add(name,reference,comment)
    .Request()
    .PostAsync();

```