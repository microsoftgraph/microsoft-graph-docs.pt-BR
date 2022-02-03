---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7877fce2c90fa8e3054077296a2e5bc45da55dfa
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352737"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Description = "Lyn Damer play in the Women's 1st Division (Toppserien) in Norway"
}

# A UPN can also be used as -UserId.
Update-MgUserProfileWebsite -UserId $userId -PersonWebsiteId $personWebsiteId -BodyParameter $params

```