---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e78ef690ff4e93542fc8ea5b6bb4e9c97dbcb28d
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352099"
---
```powershell

Import-Module Microsoft.Graph.Mail

# A UPN can also be used as -UserId.
Get-MgUserMailFolderMessage -UserId $userId -MailFolderId $mailFolderId

```