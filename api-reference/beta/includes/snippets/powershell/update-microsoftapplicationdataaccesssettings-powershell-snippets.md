---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 89dffb7c04f1216869fd4b63aeed1ea390fe9d41
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212389"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    DisabledForGroup = "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}

Update-MgOrganizationSettingMicrosoftApplicationDataAccess -OrganizationId $organizationId -BodyParameter $params

```