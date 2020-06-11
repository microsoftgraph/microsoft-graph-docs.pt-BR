---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 85f3d7e3f2e19ce748dc952f5dc6bc19f9369afa
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44682206"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"]
    .DataBodyRange()
    .Request()
    .GetAsync();

```