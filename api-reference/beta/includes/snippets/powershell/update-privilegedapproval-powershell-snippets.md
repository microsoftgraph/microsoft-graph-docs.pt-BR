---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 347c8d549ff1637812ab35758409a46401793c3c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135396"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    ApprovalState = "approvalState-value"
    ApproverReason = "approverReason-value"
}

Update-MgPrivilegedApproval -PrivilegedApprovalId $privilegedApprovalId -BodyParameter $params

```