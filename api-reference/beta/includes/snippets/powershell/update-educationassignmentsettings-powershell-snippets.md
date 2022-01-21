---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c2fc6a1bc2ff0f73d5064adbebe10d2dedefa7f7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62133710"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    SubmissionAnimationDisabled = $true
}

Update-MgEducationClassAssignmentSetting -EducationClassId $educationClassId -BodyParameter $params

```