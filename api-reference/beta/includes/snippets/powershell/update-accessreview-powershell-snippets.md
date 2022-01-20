---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d92f454ed7cd220ddd85f1f1e7fa78dc9bcb8908
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62107190"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    DisplayName = "TestReview new name"
}

Update-MgAccessReview -AccessReviewId $accessReviewId -BodyParameter $params

```