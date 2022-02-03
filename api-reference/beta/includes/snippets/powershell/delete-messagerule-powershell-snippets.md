---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bb249ea196c132896fa894fa23bccc3cdbb8a9e9
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351452"
---
```powershell

Import-Module Microsoft.Graph.Mail

# A UPN can also be used as -UserId.
Remove-MgUserMailFolderMessageRule -UserId $userId -MailFolderId $mailFolderId -MessageRuleId $messageRuleId

```