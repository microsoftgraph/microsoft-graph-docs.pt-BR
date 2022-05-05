---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 27612617ec36b261c9508478bd32d5ddbb4d69ab
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220235"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    DisplayName = "Azure AD SAML Toolkit"
}

Invoke-MgInstantiateApplicationTemplate -ApplicationTemplateId $applicationTemplateId -BodyParameter $params

```