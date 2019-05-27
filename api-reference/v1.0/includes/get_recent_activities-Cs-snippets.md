---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bcaab345dffb05ab00cfda6bf015ac1a94bd2ce6
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34466764"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var recent = await graphClient.Me.Activities.Recent()
    .Request()
    .GetAsync();

```