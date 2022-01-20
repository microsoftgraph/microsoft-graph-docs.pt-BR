---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fd800f92852481ffccd85af67c70aab3806e5a2e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62115608"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgInformationProtectionThreatAssessmentRequest -ThreatAssessmentRequestId $threatAssessmentRequestId -ExpandProperty "results" 

```