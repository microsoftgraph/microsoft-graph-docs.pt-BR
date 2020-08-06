---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ae63e4b2ca3fb23082e2f2fcd656f1f180c48541
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565016"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.ConditionalAccess.NamedLocations["0854951d-5fc0-4eb1-b392-9b2c9d7949c2"]
    .Request()
    .DeleteAsync();

```