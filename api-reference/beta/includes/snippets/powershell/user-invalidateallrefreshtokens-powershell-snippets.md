---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 97ab90565594d51e4f321a3d0741ab36d21a0914
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62339136"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

# A UPN can also be used as -UserId.
Invoke-MgInvalidateUserRefreshToken -UserId $userId

```