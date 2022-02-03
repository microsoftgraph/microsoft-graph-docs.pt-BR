---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 089e3c0503fd76f898e77272cc833e9bfb928e57
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350029"
---
```powershell

Import-Module Microsoft.Graph.Mail

# A UPN can also be used as -UserId.
Get-MgUserMessageContent -UserId $userId -MessageId $messageId

```