---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b94917cca868e3b9a1fefc0112f86442d5a521be
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349334"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfileAward -UserId $userId -PersonAwardId $personAwardId

```