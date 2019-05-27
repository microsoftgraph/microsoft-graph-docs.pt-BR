---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3b0d05b4c0a9df13a0ae16d56704747a4d30a07d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474034"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var applicationSignInDetailedSummary = await graphClient.Reports.ApplicationSignInDetailedSummary["'id'"]
    .Request()
    .GetAsync();

```