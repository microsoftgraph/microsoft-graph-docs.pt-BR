---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d0f12477659e0b76125ffaedd1b7b7ca4ca913b3
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343274"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

# A UPN can also be used as -UserId.
New-MgUserMessageReplyAll -UserId $userId -MessageId $messageId

```