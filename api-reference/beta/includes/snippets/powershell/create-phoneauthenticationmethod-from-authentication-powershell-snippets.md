---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5ba11010a2fe0741334c324aaa03a880cc01745e
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349490"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    PhoneNumber = "+1 2065555555"
    PhoneType = "mobile"
}

# A UPN can also be used as -UserId.
New-MgUserAuthenticationPhoneMethod -UserId $userId -BodyParameter $params

```