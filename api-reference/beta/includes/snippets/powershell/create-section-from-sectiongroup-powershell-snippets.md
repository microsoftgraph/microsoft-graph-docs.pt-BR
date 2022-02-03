---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4135071cbbf4258b26b8da88ad582421a6cdddc2
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352065"
---
```powershell

Import-Module Microsoft.Graph.Notes

$params = @{
    DisplayName = "Section name"
}

# A UPN can also be used as -UserId.
New-MgUserOnenoteSectionGroupSection -UserId $userId -SectionGroupId $sectionGroupId -BodyParameter $params

```