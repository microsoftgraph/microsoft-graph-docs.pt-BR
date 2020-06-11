---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f60e138f19338a70f7ce15cff7e358d0fe866cb5
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684887"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var rooms = await graphClient.Places["bldg2@contoso.com"].Rooms
    .Request()
    .GetAsync();

```