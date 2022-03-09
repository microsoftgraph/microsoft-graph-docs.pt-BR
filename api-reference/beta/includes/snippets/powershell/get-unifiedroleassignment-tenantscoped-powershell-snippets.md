---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e5fa5a175ac28fdc2e6b8c5f8f3fdebc5923fa9f
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63396298"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Enrolment

Get-MgRoleManagementDirectoryTransitiveRoleAssignment -CountVariable CountVar -Filter "principalId eq '2c7936bc-3517-40f3-8eda-4806637b6516' and directoryScopeId eq '/administrativeUnits/26e79164-0c5c-4281-8c5b-be7bc7809fb2'" 

```