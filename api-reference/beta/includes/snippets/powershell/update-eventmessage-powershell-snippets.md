---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5a2737d8832500c517bed803255de9ad1e11b989
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135551"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    IsRead = "true"
}

Update-MgUserMessage -UserId $userId -MessageId $messageId -BodyParameter $params

```