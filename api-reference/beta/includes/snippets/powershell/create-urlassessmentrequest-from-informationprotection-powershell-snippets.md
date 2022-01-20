---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 12707a8e8a9952b029bfbf3530fbc5a1ab0ae9be
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094046"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    "@odata.type" = "#microsoft.graph.urlAssessmentRequest"
    Url = "http://test.com"
    ExpectedAssessment = "block"
    Category = "phishing"
}

New-MgInformationProtectionThreatAssessmentRequest -BodyParameter $params

```