---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cd8a5ddb4d658b05498d1033c28482dd1da075f0
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347690"
---
```powershell

Import-Module Microsoft.Graph.Compliance

$params = @{
    OutputName = "2020-12-06 Contoso investigation export"
    Description = "Export for the Contoso investigation"
    ExportOptions = "originalFiles,fileInfo,tags"
    ExportStructure = "directory"
}

Export-MgComplianceEdiscoveryCaseReviewSet -CaseId $caseId -ReviewSetId $reviewSetId -BodyParameter $params

```