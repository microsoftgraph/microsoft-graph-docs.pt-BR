---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b73132f73b1d958f583a0b7d1177ceb513fe979b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62122082"
---
```powershell

Import-Module Microsoft.Graph.Mail

Remove-MgUserMailFolderMessageRule -UserId $userId -MailFolderId $mailFolderId -MessageRuleId $messageRuleId

```