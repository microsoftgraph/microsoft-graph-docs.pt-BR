---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0960d31ba3636a2477da3b473e7c1341b3879ca9
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63333061"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

Get-MgEntitlementManagementAccessPackageAssignmentPolicy -AccessPackageAssignmentPolicyId $accessPackageAssignmentPolicyId -ExpandProperty "customExtensionHandlers(`$expand=customExtension)" 

```