---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c09fdc2b1b214ec74b9bdaf22a8600b07ab00732
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132772"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Categories = @(
        "Professional"
    )
    AllowedAudiences = "organization"
    DisplayName = "API Design"
    Proficiency = "generalProfessional"
    CollaborationTags = @(
        "ableToMentor"
    )
}

New-MgUserProfileSkill -UserId $userId -BodyParameter $params

```