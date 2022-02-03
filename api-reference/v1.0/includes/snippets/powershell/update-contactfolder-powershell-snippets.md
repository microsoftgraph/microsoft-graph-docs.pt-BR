---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 038c997343ee7124effcb426cc0361598a870d49
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351039"
---
```powershell

Import-Module Microsoft.Graph.PersonalContacts

$params = @{
    ParentFolderId = "parentFolderId-value"
    DisplayName = "displayName-value"
}

# A UPN can also be used as -UserId.
Update-MgUserContactFolder -UserId $userId -ContactFolderId $contactFolderId -BodyParameter $params

```