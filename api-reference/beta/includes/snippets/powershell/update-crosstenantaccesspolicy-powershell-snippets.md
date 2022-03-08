---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 999672bab7d8772cb97bd999e80b45c8a0658f3e
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336645"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    DisplayName = "CrossTenantAccessPolicy"
}

Update-MgPolicyCrossTenantAccessPolicy -BodyParameter $params

```