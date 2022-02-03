---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 190c4c1597f415e105a6bf4a77e2aa1d707ea763
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348015"
---
```powershell

Import-Module Microsoft.Graph.Users.Functions

# A UPN can also be used as -UserId.
Invoke-MgRecentUserActivity -UserId $userId

```