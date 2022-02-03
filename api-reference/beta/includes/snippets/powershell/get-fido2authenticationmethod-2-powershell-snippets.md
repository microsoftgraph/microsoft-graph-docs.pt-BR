---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 80f5e1e0e018c34a07141eb8a3aef9f9d8db7de5
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350335"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

# A UPN can also be used as -UserId.
Get-MgUserAuthenticationFido2Method -UserId $userId

```