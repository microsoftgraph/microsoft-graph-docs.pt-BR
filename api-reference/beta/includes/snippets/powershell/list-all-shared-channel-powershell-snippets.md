---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 711ecbd0b2781897f98bb4f4c45e8537c0d7c057
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212549"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgTeamChannel -TeamId $teamId -Filter "membershipType eq 'shared'" 

```