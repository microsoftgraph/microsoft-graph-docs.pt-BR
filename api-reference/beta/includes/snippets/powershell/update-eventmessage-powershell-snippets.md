---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e4bd142df2a66ac6ad680db9ebc2f80ea2625b2f
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350719"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    IsRead = "true"
}

# A UPN can also be used as -UserId.
Update-MgUserMessage -UserId $userId -MessageId $messageId -BodyParameter $params

```