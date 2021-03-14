---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 497a33bb861ca746f50cabad5078c70f95691c58
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801256"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var rooms = await graphClient.Places["{place-id}"].Rooms
    .Request()
    .GetAsync();

```