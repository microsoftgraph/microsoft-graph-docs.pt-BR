---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6fd43cbdb92e3c84cb54b63ddfc4cd3e6bd1357d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136160"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    ExternalUserLifecycleAction = "None"
}

Update-MgEntitlementManagementSetting -BodyParameter $params

```