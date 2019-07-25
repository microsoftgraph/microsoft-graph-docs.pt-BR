---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b8ee54595523d2618e2dd93a72282cb4e59f23eb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871939"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessParticipantActivityUserCounts = await graphClient.Reports
    .GetSkypeForBusinessParticipantActivityUserCounts('D7')
    .Request()
    .GetAsync();

```