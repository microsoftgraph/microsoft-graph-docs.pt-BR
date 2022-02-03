---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 832f183d31e2d1bd09b905d57949a39f452bc335
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350953"
---
```powershell

Import-Module Microsoft.Graph.Mail

# A UPN can also be used as -UserId.
Remove-MgUserMailFolder -UserId $userId -MailFolderId $mailFolderId

```