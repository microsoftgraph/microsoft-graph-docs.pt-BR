---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 088decec2c2000e349a86d4bb6113f385c074b22
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351086"
---
```powershell

Import-Module Microsoft.Graph.CrossDeviceExperiences

# A UPN can also be used as -UserId.
Remove-MgUserActivity -UserId $userId -UserActivityId $userActivityId

```