---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bb5fe6ac188762ffe0ceae73c6b69bc827b0e1be
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34469234"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var timeOff = await graphClient.Teams["{teamId}"].Schedule.TimesOff["{timeOffId}"]
    .Request()
    .GetAsync();

```