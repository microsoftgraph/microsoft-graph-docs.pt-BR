---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6fa67d4c7b600257adab9b6400136a314766fe80
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62089395"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgTeamMember -TeamId $teamId -Filter "roles/any(r:r eq 'owner')" 

```