---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 79a7a6b1f29e5b17131b86fcd787e60ce09b15ec
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34441945"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getMailboxUsageMailboxCounts = await graphClient.Reports.GetMailboxUsageMailboxCounts('D7')
    .Request()
    .GetAsync();

```