---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 96076d4f3639b45eff5d99ce1e2f68a2443d2616
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62109291"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    PolicyViolation = @{
        PolicyTip = @{
            GeneralText = "This item has been blocked by the administrator."
            ComplianceUrl = "https://contoso.com/dlp-policy-page"
            MatchedConditionDescriptions = @(
                "Credit Card Number"
            )
        }
        VerdictDetails = "AllowOverrideWithoutJustification,AllowFalsePositiveOverride"
        DlpAction = "BlockAccess"
    }
}

Update-MgTeamChannelMessage -TeamId $teamId -ChannelId $channelId -ChatMessageId $chatMessageId -BodyParameter $params

```