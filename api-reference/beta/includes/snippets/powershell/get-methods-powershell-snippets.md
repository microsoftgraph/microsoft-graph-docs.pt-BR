---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: daa7908995aa3f40cd17825f838a41c649a55a47
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351821"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

# A UPN can also be used as -UserId.
Get-MgUserAuthenticationMethod -UserId $userId

```