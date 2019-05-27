---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1610f13e68f41ed9adc9108f3dffd8c6265a2cb0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463866"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessPeerToPeerActivityUserCounts = await graphClient.Reports.GetSkypeForBusinessPeerToPeerActivityUserCounts('D7')
    .Request()
    .GetAsync();

```