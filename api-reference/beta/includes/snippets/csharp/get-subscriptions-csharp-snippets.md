---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 340db99262c2c9d3473c9c32f990888433be36ee
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518753"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subscriptions = await graphClient.Subscriptions
    .Request()
    .GetAsync();

```