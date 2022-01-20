---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 64ab6f0cff528dac027a4cbdf30c343200bee7c4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094043"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    "@odata.type" = "#microsoft.graph.fileAssessmentRequest"
    ExpectedAssessment = "block"
    Category = "malware"
    FileName = "test.txt"
    ContentData = "VGhpcyBpcyBhIHRlc3QgZmlsZQ=="
}

New-MgInformationProtectionThreatAssessmentRequest -BodyParameter $params

```