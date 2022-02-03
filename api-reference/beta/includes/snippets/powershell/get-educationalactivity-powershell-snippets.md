---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 165af452029baeeac5a3887a80706da6d65d6a3b
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351224"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfileEducationalActivity -UserId $userId -EducationalActivityId $educationalActivityId

```