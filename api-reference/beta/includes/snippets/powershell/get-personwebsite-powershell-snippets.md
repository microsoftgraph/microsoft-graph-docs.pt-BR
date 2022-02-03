---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1210e62895e9f0e15aa05595d2a22a980d85ad65
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351182"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfileWebsite -UserId $userId -PersonWebsiteId $personWebsiteId

```