---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3acc68149bc7429cb31ac94380d4b1f303307a8f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62127935"
---
```powershell

Import-Module Microsoft.Graph.Compliance

$params = @{
    "@odata.type" = "microsoft.graph.ediscovery.siteSource"
}

New-MgComplianceEdiscoveryCaseSourceCollectionAdditionalSource -CaseId $caseId -SourceCollectionId $sourceCollectionId -BodyParameter $params

```