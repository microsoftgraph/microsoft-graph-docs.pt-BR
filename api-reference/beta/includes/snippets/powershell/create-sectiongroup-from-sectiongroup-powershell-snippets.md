---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fbea2c86c460e1897172dd0fd9529f77b802cc18
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350660"
---
```powershell

Import-Module Microsoft.Graph.Notes

$params = @{
    DisplayName = "Section group name"
}

# A UPN can also be used as -UserId.
New-MgUserOnenoteSectionGroup -UserId $userId -SectionGroupId $sectionGroupId -BodyParameter $params

```