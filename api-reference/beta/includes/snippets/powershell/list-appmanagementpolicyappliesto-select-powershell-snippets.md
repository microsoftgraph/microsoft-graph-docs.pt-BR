---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a1fa88870a0f0e06fbcd014c7c06e27583fdc50b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62114440"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgPolicyAppManagementPolicyApplyTo -AppManagementPolicyId $appManagementPolicyId -Property "id,appId,displayName,createdDateTime" 

```