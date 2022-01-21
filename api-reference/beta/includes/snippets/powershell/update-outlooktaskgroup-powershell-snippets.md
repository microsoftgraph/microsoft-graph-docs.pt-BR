---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 01a174593a925d98a5e873381b550864f51deb8a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62099140"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    Name = "Personal Tasks"
}

Update-MgUserOutlookTaskGroup -UserId $userId -OutlookTaskGroupId $outlookTaskGroupId -BodyParameter $params

```