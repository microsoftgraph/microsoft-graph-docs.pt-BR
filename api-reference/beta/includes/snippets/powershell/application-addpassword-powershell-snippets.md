---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 46634cfc1481bcbee042d683239ab6c7b47d58d4
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62339380"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    PasswordCredential = @{
        DisplayName = "Password friendly name"
    }
}

Add-MgApplicationPassword -ApplicationId $applicationId -BodyParameter $params

```