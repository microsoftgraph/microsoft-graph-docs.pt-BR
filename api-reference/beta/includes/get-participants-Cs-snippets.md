---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e7f12dbc19a85b50c58ddcb69e24b7ad05edec1a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34435940"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var participants = await graphClient.App.Calls["57DAB8B1894C409AB240BD8BEAE78896"].Participants
    .Request()
    .Header("Authorization","Bearer <TOKEN>")
    .GetAsync();

```