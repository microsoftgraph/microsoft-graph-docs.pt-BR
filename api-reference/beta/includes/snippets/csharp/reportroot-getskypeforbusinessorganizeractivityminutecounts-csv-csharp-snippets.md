---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 17591d43583e94bb2cc06946589eba12f702c699
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872175"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessOrganizerActivityMinuteCounts = await graphClient.Reports
    .GetSkypeForBusinessOrganizerActivityMinuteCounts('D7')
    .Request()
    .GetAsync();

```