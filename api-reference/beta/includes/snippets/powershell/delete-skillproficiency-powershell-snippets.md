---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e4c866b1154ea8aa68e48c1fd2210f466454cf71
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351384"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Remove-MgUserProfileSkill -UserId $userId -SkillProficiencyId $skillProficiencyId

```