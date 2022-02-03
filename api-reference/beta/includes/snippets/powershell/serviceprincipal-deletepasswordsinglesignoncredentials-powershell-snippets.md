---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0264b5f36d86a7bf11995344dd5f10c0aa514e3e
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62345499"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    Id = "5793aa3b-cca9-4794-679a240f8b58"
}

Remove-MgServicePrincipalPasswordSingleSignOnCredentials -ServicePrincipalId $servicePrincipalId -BodyParameter $params

```