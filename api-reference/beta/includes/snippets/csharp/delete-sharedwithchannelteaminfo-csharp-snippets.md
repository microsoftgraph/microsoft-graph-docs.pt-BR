---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6c6ce200e1200e86a4a595fc408a47c1a1fdfaa2
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2022
ms.locfileid: "65628902"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"].Channels["{channel-id}"].SharedWithTeams["{sharedWithChannelTeamInfo-id}"]
    .Request()
    .DeleteAsync();

```