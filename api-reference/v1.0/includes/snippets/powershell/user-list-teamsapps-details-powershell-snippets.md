---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b753d5d0cd73f44a3746f6b6fbeafa6e61814a8f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62087556"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgUserTeamworkInstalledApp -UserId $userId -ExpandProperty "teamsAppDefinition" 

```