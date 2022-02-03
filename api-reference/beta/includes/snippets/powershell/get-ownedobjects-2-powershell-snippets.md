---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 838bacccb009dcb8e80563b1683981104b290235
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351104"
---
```powershell

Import-Module Microsoft.Graph.Users

# A UPN can also be used as -UserId.
Get-MgUserOwnedObject -UserId $userId

```