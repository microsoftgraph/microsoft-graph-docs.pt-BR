---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: de40f4da6aae7092784e7528db507db83025b955
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350634"
---
```powershell

Import-Module Microsoft.Graph.Mail

# A UPN can also be used as -UserId.
Get-MgUserMessage -UserId $userId -Property "sender,subject" 

```