---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5f2bae6dc8380bc92792382c9b0b272b423a4b49
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62342040"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

# A UPN can also be used as -UserId.
Invoke-MgUnsubscribeUserMessage -UserId $userId -MessageId $messageId

```