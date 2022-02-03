---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f31e28af9e19c58b6b83a3fd97c4b737068c2a76
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351890"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Remove-MgUserProfileInterest -UserId $userId -PersonInterestId $personInterestId

```