---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4b24b5108a9b1622c583d83f57dd24e584584775
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129643"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Categories = @(
        "Sports"
    )
}

Update-MgUserProfileInterest -UserId $userId -PersonInterestId $personInterestId -BodyParameter $params

```