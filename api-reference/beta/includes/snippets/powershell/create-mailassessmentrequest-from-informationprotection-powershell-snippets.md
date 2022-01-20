---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c38018b14c2d6c9a4124f0b35398825052d50d60
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094047"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    "@odata.type" = "#microsoft.graph.mailAssessmentRequest"
    RecipientEmail = "tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com"
    ExpectedAssessment = "block"
    Category = "spam"
    MessageUri = "https://graph.microsoft.com/beta/users/c52ce8db-3e4b-4181-93c4-7d6b6bffaf60/messages/AAMkADU3MWUxOTU0LWNlOTEt="
}

New-MgInformationProtectionThreatAssessmentRequest -BodyParameter $params

```