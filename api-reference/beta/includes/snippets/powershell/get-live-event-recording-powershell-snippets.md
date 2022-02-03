---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 79c14e0a81316f64bfee7acac98021e95427a99c
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352508"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

# A UPN can also be used as -UserId.
Get-MgUserOnlineMeetingRecording -UserId $userId -OnlineMeetingId $onlineMeetingId

```