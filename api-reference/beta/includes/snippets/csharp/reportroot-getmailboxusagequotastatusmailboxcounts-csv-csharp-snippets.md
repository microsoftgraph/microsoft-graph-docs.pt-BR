---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 469c0ce2e847181b58b3205b6209724fa5d1a066
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35477022"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getMailboxUsageQuotaStatusMailboxCounts = await graphClient.Reports.GetMailboxUsageQuotaStatusMailboxCounts('D7')
    .Request()
    .GetAsync();

```