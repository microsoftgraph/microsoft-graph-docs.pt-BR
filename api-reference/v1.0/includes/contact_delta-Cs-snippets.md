---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a9c3ee3d03126a4452533aafc3ea9afd69f713a6
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34467086"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.ContactFolders["{id}"].Contacts.Delta()
    .Request()
    .Header("Prefer","odata.maxpagesize=2")
    .Select( e => new {
             e.DisplayName 
             })
    .GetAsync();

```