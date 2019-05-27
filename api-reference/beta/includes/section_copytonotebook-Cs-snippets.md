---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6253573e4713824e1bcfb7e24389c42633515778
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480404"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var id = "id-value";

var groupId = "groupId-value";

var renameAs = "renameAs-value";

await graphClient.Me.Onenote.Sections["{id}"]
    .CopyToNotebook(id,groupId,renameAs,siteCollectionId,siteId)
    .Request()
    .PostAsync();

```