---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6d7dc666097631ec7a983b6019623731528d33ed
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2022
ms.locfileid: "63527997"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    DisplayName = "All Contoso volunteers - Terms of use"
    IsViewingBeforeAcceptanceRequired = $true
}

Update-MgIdentityGovernanceTermOfUseAgreement -AgreementId $agreementId -BodyParameter $params

```