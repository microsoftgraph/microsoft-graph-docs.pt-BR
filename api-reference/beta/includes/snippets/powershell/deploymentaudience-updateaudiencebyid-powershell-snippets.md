---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ada85e32911f6fc26fc94ab338bc1dd6e77acc23
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62342510"
---
```powershell

Import-Module Microsoft.Graph.WindowsUpdates

$params = @{
    MemberEntityType = "String"
    AddMembers = @(
        "String"
    )
    RemoveMembers = @(
        "String"
    )
    AddExclusions = @(
        "String"
    )
    RemoveExclusions = @(
        "String"
    )
}

Update-MgWindowsUpdatesDeploymentAudienceById -DeploymentId $deploymentId -BodyParameter $params

```