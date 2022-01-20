---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c46b40bd1367ba9ea1737c962733d0d93cb0a55e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62133653"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    "@odata.id" = "https://graph.microsoft.com/beta/education/users/14008"
}

New-MgEducationSchoolUserByRef -EducationSchoolId $educationSchoolId -BodyParameter $params

```