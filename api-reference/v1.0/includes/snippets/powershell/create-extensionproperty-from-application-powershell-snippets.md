---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7ffbe816e6771eac4934d56a5b5cc355ca4b6bb8
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411337"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    Name = "jobGroup"
    DataType = "String"
    TargetObjects = @(
        "User"
    )
}

New-MgApplicationExtensionProperty -ApplicationId $applicationId -BodyParameter $params

```