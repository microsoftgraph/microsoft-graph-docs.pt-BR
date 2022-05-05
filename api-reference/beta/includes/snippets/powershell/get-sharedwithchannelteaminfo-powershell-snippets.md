---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b48a7af218176cd490947c1ab275325bf2601348
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212430"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgTeamChannelShared -TeamId $teamId -ChannelId $channelId -SharedWithChannelTeamInfoId $sharedWithChannelTeamInfoId

```