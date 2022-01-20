---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 29d886a8d3b95fcf5f9e95b341310c4f9d712d34
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62121130"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    "@odata.id" = "https://graph.microsoft.com/onPremisesPublishingProfiles/applicationproxy/connectorGroups/{id}"
}

Set-MgApplicationConnectorGroupByRef -ApplicationId $applicationId -BodyParameter $params

```