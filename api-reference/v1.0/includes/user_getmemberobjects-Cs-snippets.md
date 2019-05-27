---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 33f9d42a98d86a655d9644d3150c9c591244b79f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34466664"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = true;

await graphClient.Me
    .GetMemberObjects(securityEnabledOnly)
    .Request()
    .PostAsync();

```