---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b31e0f54737b9760e30140c22e54d18f0b74691a
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684217"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var content = await graphClient.Me.Drive.Items["{item-id}"].Thumbnails["{thumb-id}"]["{size}"].Content
    .Request()
    .GetAsync();

```