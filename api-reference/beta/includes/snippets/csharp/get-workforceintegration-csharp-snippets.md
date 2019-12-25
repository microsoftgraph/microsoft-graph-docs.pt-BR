---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7274f06fcd816db0da48be70cf6fa6a46bb63d86
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870522"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workforceIntegration = await graphClient.Teamwork.WorkforceIntegrations["{workforceintegrationid}"]
    .Request()
    .GetAsync();

```