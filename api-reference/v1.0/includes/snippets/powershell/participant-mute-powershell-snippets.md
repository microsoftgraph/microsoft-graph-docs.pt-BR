---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9c46b32668836298722c909eb60654787e18f8a9
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62346232"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    ClientContext = "d45324c1-fcb5-430a-902c-f20af696537c"
}

Invoke-MgMuteCommunicationCallParticipant -CallId $callId -ParticipantId $participantId -BodyParameter $params

```