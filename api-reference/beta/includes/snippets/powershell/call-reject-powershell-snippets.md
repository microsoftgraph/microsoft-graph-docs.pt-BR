---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 662f4deb2ce3b3f018039ff306bfef70bb60e6c3
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340308"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    Reason = "busy"
}

Invoke-MgRejectCommunicationCall -CallId $callId -BodyParameter $params

```