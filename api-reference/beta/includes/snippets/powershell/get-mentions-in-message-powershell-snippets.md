---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b3f0bb1c5c01e466f77d4e3442424cfa7ccafbf2
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351053"
---
```powershell

Import-Module Microsoft.Graph.Mail

# A UPN can also be used as -UserId.
Get-MgUserMessage -UserId $userId -MessageId $messageId -ExpandProperty "mentions" 

```