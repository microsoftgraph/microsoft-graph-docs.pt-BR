---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 17e5395e33ddcdec714be3267fbedab640b06c9f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320620"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSkypeForBusinessPeerToPeerActivityCounts("D7")
    .Request()
    .GetAsync();

```