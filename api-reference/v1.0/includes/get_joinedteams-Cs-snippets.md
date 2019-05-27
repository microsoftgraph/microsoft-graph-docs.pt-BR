---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fa6ace24c4504393915499730b35f04037500ee3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34457203"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var joinedTeams = await graphClient.Me.JoinedTeams
    .Request()
    .GetAsync();

```