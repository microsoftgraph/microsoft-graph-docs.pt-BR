---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0e97354f22c15d17bac3dcf40b61a741fc37c56c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62089667"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    Name = "Charity work"
}

Update-MgUserOutlookTaskFolder -UserId $userId -OutlookTaskFolderId $outlookTaskFolderId -BodyParameter $params

```