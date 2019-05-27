---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d73dbe112c680a3e3fa0a5ea0c69ad0e46aae649
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444171"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var destinationId = "destinationId-value";

await graphClient.Me.MailFolders["{id}"]
    .Move(destinationId)
    .Request()
    .PostAsync();

```