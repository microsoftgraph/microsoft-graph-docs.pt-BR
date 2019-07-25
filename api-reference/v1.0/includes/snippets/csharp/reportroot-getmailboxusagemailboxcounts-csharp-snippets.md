---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: caf025044f93adec7be556a62aa8a25f3d4f14a0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35894373"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetMailboxUsageMailboxCounts('D7')
    .Request()
    .GetAsync();

```