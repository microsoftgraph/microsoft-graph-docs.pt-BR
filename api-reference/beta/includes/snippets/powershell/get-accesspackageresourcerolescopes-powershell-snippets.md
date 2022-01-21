---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2dd00120d8df5574bae664b421e97a43b14a07a1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62104103"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

Get-MgEntitlementManagementAccessPackage -AccessPackageId $accessPackageId -ExpandProperty "accessPackageResourceRoleScopes(`$expand=accessPackageResourceRole,accessPackageResourceScope)" 

```