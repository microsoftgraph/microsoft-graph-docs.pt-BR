---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2f7ede6240351e046a503e8a0db7c2ccdd07d207
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684451"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var room = await graphClient.Places
    .Request()
    .GetAsync();

```