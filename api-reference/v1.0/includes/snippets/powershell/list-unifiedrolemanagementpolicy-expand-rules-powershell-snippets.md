---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9ffc440a3a5bf1cbe48ba3c227839b299eb29a87
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66442182"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgPolicyRoleManagementPolicy -Filter "scopeId eq '/' and scopeType eq 'Directory'" -ExpandProperty "rules" 

```