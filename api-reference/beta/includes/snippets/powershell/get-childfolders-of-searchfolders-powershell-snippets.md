---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 411c0843e9fa0da1e4f6d0e013bb4b921ab21b68
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349391"
---
```powershell

Import-Module Microsoft.Graph.Mail

# A UPN can also be used as -UserId.
Get-MgUserMailFolderChildFolder -UserId $userId -MailFolderId $mailFolderId

```