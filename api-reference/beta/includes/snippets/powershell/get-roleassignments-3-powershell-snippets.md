---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dd07bc65c4c57cbb320397ca3463d5faa1ba4b9e
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63396515"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Enrolment

Get-MgRoleManagementEntitlementManagementRoleAssignment -Filter "appScopeId eq '/AccessPackageCatalog/4cee616b-fdf9-4890-9d10-955e0ccb12bc'" -ExpandProperty "principal" 

```