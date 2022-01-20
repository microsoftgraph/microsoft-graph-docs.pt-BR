---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 36f4c1f2444d18ec61208f650ec6ef8184aab647
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094919"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    Value = @(
    )
}

Update-MgIdentityConditionalAccessAuthenticationContextClassReference -AuthenticationContextClassReferenceId $authenticationContextClassReferenceId -BodyParameter $params

```