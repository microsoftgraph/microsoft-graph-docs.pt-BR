---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 836bcb4197ed3eed4f3a8235e656a6b3ede0b21a
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351702"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Remove-MgUserProfileEducationalActivity -UserId $userId -EducationalActivityId $educationalActivityId

```