---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 17ded7b4788f75eb8a5575d756ebaa623b6ea38e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62133177"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Remove-MgUserAuthenticationPhoneMethod -UserId $userId -PhoneAuthenticationMethodId $phoneAuthenticationMethodId

```