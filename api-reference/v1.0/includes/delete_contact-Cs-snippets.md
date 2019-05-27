---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f3d2d87bb866e31946c2486ea8074b7e0a1d6482
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459495"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Contacts["{id}"]
    .Request()
    .DeleteAsync();

```