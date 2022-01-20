---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 484bd6c67d89cdfabb7c52b11f3cb13537aa98e6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62117974"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    IsEnabled = "false"
}

Update-MgUserSettingItemInsight -UserId $userId -BodyParameter $params

```