---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1580bf655c6720528cb776135e69d19a3133466c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358720"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getTeamsUserActivityUserDetail = await graphClient.Reports
    .GetTeamsUserActivityUserDetail("D7")
    .Request()
    .GetAsync();

```