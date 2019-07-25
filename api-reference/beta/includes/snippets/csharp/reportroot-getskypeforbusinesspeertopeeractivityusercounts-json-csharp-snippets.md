---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 23f0d1692c33596fe2dd4bbbb7ca643f92aec56d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871882"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessPeerToPeerActivityUserCounts = await graphClient.Reports
    .GetSkypeForBusinessPeerToPeerActivityUserCounts('D7')
    .Request()
    .GetAsync();

```