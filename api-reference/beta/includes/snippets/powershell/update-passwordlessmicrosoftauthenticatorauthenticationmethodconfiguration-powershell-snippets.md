---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 28e56d455afd7953c6caea18b154e97f3d0fe3b4
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66439961"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    "@odata.type" = "#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration"
    State = "enabled"
}

Update-MgPolicyAuthenticationMethodPolicyAuthenticationMethodConfiguration -AuthenticationMethodConfigurationId $authenticationMethodConfigurationId -BodyParameter $params

```