---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7855fbf3bc9fb4c03063c2cc41de033349b64d2a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34453283"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Security.SecurityActions["{id}"]
    .CancelSecurityAction()
    .Request()
    .PostAsync();

```