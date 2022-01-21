---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a118fd471e81ba59dfe6a995c8a0776c6f39d828
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62097102"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    Name = "name-value"
    Region = "region-value"
}

Update-MgOnPremisePublishingProfileConnectorGroup -OnPremisesPublishingProfileId $onPremisesPublishingProfileId -ConnectorGroupId $connectorGroupId -BodyParameter $params

```