---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5c6cadd0acd0d310fd9a6a31a1e1bb17a0428453
ms.sourcegitcommit: ab36e03d6bcb5327102214eb078d55709579d465
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/11/2020
ms.locfileid: "45224796"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Devices["{id}"].RegisteredUsers["{id}"].Reference
    .Request()
    .DeleteAsync();

```