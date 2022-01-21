---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ad6a049f04c372cbf95d511130374be2a1b6de91
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116776"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    PhoneNumber = "+1 2065555555"
    PhoneType = "mobile"
}

New-MgUserAuthenticationPhoneMethod -UserId $userId -BodyParameter $params

```