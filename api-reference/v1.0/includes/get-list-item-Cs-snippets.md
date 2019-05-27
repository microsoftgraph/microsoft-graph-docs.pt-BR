---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 83718b8cacd6f964cda5f766a8c734b729b79557
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480194"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var listItem = await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items["{item-id}"]
    .Request()
    .GetAsync();

```