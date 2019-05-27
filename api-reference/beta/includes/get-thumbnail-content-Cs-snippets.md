---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 273921dab668b5b947287cbbd82e7889da1ddc5c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474517"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var content = await graphClient.Me.Drive.Items["{item-id}"].Thumbnails["{thumb-id}"].{size}.Content
    .Request()
    .GetAsync();

```