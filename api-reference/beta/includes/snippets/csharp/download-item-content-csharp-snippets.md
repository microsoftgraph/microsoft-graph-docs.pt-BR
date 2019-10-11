---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7917930b7b44256614d2d5b118b53bb93f585a1b
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428705"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Me.Drive.Items["{item-id}"].Content
    .Request()
    .GetAsync();

```