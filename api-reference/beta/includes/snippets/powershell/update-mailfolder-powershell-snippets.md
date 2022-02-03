---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f2cff9e84dadee26770128bccd5f51ff7465d8a5
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352286"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    DisplayName = "displayName-value"
}

# A UPN can also be used as -UserId.
Update-MgUserMailFolder -UserId $userId -MailFolderId $mailFolderId -BodyParameter $params

```