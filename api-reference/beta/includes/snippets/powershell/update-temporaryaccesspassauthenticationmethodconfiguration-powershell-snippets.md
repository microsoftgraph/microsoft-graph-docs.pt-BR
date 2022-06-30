---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e35069e4dffa869e6f7c8049381f628bbc90b208
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66442739"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    "@odata.type" = "#microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration"
    IsUsableOnce = $true
}

Update-MgPolicyAuthenticationMethodPolicyAuthenticationMethodConfiguration -AuthenticationMethodConfigurationId $authenticationMethodConfigurationId -BodyParameter $params

```