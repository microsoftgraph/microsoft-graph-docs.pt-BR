---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a8e939fa2770105932aff60e30f06f7e7b1987f2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62127417"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    "@odata.type" = "microsoft.graph.mailSearchFolder"
    FilterQuery = "contains(subject, 'Analytics')"
}

Update-MgUserMailFolder -UserId $userId -MailFolderId $mailFolderId -BodyParameter $params

```