---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a722667b3746c837d063ce538b3c2310a0ace684
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352116"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

# A UPN can also be used as -UserId.
Get-MgUserAuthenticationPasswordlessMicrosoftAuthenticatorMethod -UserId $userId

```