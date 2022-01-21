---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: abcc209ee1084c3be943602be6bb3ac8f693a51e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62098138"
---
```powershell

Import-Module Microsoft.Graph.PersonalContacts

$params = @{
    ParentFolderId = "parentFolderId-value"
    DisplayName = "displayName-value"
}

Update-MgUserContactFolder -UserId $userId -ContactFolderId $contactFolderId -BodyParameter $params

```