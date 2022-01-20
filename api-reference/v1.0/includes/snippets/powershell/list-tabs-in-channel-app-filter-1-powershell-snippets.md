---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b142ea79e7a1b95692c59cedf753d4030d0ff562
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62104973"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgTeamChannelTab -TeamId $teamId -ChannelId $channelId -ExpandProperty "teamsApp" 

```