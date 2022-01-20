---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 59b873a35572ed871c98594846a69859cd1aa970
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100687"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    IsGroupOwnerManagementEnabled = $true
}

Update-MgPolicyAccessReviewPolicy -BodyParameter $params

```