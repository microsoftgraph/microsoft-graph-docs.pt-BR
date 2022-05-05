---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 619db03cd890e09d33aae5e62c9655815579b35a
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203777"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

Get-MgEntitlementManagementAccessPackageAssignment -AccessPackageAssignmentId $accessPackageAssignmentId -ExpandProperty "target" 

```