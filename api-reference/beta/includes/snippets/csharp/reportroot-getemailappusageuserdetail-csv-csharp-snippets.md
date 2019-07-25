---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 119eea954e0799b0032afa9972f228cea95d971c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873842"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getEmailAppUsageUserDetail = await graphClient.Reports
    .GetEmailAppUsageUserDetail('D7')
    .Request()
    .GetAsync();

```