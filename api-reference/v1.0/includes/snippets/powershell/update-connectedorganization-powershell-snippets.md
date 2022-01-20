---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b904a3481e7354c12dc57ce2d2033cb563c59496
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62122237"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    DisplayName = "Connected organization new name"
    Description = "Connected organization new description"
    State = "configured"
}

Update-MgEntitlementManagementConnectedOrganization -ConnectedOrganizationId $connectedOrganizationId -BodyParameter $params

```