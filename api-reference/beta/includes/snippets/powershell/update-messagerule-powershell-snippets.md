---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ca9bd227ca2a8af55ae621ebdf1753623227baf4
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351364"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    DisplayName = "Important from partner"
    Actions = @{
        MarkImportance = "high"
    }
}

# A UPN can also be used as -UserId.
Update-MgUserMailFolderMessageRule -UserId $userId -MailFolderId $mailFolderId -MessageRuleId $messageRuleId -BodyParameter $params

```