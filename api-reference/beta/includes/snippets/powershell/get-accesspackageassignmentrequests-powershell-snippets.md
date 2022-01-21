---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 866e8d7062684be273ed74b22ebdfc398e7453a3
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113634"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

Get-MgEntitlementManagementAccessPackageAssignmentRequest -ExpandProperty "requestor(`$expand=connectedOrganization)" -Filter "(requestState eq 'PendingApproval')" 

```