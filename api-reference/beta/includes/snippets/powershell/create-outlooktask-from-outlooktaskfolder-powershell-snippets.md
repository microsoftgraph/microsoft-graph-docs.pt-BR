---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 173fd3d5acd2f0ec72a60ce756250113cfec30ac
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62089695"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    Subject = "Shop for dinner"
    StartDateTime = @{
        DateTime = "2016-04-23T18:00:00"
        TimeZone = "Pacific Standard Time"
    }
    DueDateTime = @{
        DateTime = "2016-04-25T13:00:00"
        TimeZone = "Pacific Standard Time"
    }
}

New-MgUserOutlookTaskFolderTask -UserId $userId -OutlookTaskFolderId $outlookTaskFolderId -BodyParameter $params

```