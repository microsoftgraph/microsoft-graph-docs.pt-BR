---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f3170217cb3e0e876c00e543e062ac286b62d013
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349779"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfileLanguage -UserId $userId -LanguageProficiencyId $languageProficiencyId

```