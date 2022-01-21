---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c96577d1e06aaa0aaa1ab99c79482714cdafacc1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62096304"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    DisplayName = "Business Email"
    Type = "work"
}

Update-MgUserProfileEmail -UserId $userId -ItemEmailId $itemEmailId -BodyParameter $params

```