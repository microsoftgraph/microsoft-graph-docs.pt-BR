---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a5020d8334f5b58ca643a85731a4356275f0c67c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35508186"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"]
    .ConvertToRange()
    .Request()
    .PostAsync();

```