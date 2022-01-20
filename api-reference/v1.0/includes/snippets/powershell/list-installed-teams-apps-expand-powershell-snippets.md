---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 84a90cdf228ab7b3b270c2dfcba78f909ba4707f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62121798"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgTeamInstalledApp -TeamId $teamId -ExpandProperty "teamsAppDefinition" 

```