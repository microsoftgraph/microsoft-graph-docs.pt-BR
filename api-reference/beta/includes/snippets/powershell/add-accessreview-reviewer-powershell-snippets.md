---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5bd46f30d31655978ee498e43c1604f0ea0fcadf
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62091089"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    Id = "006111db-0810-4494-a6df-904d368bd81b"
}

New-MgAccessReviewReviewer -AccessReviewId $accessReviewId -BodyParameter $params

```