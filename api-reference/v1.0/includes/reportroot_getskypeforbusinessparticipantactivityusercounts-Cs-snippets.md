---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fbd2f275811581d162685518bb31da7129d1d015
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34457494"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetSkypeForBusinessParticipantActivityUserCounts('D7')
    .Request()
    .GetAsync();

```