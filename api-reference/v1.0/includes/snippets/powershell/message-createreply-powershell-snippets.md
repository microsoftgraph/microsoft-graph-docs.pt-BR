---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 96b795b9a90a7436f6e5ee706c1ca9bf408bb563
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62342775"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

# A UPN can also be used as -UserId.
New-MgUserMessageReply -UserId $userId -MessageId $messageId

```