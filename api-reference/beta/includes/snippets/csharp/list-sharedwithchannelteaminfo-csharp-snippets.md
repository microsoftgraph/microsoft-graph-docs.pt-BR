---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7d83601a0afe3d890c142650399b09c98cbe1614
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212775"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sharedWithTeams = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].SharedWithTeams
    .Request()
    .GetAsync();

```