---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6253573e4713824e1bcfb7e24389c42633515778
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725515"
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