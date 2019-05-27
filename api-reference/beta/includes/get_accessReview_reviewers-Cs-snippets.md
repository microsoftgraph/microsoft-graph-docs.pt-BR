---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e8184fa035985989c491300ab71b52ef41406f96
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474314"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reviewers = await graphClient.AccessReviews["2b83cc42-09db-46f6-8c6e-16fec466a82d"].Reviewers
    .Request()
    .GetAsync();

```