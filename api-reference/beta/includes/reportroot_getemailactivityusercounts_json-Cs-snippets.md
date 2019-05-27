---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4adc358ec9cd447247aafb2eca8b2b3c828b626c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34442365"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getEmailActivityUserCounts = await graphClient.Reports.GetEmailActivityUserCounts('D7')
    .Request()
    .GetAsync();

```