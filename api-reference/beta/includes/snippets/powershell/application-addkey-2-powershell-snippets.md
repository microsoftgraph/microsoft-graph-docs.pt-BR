---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 286b9d26725d4655d0c7ef4ce8fbf8ede3b8e8d5
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340463"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    KeyCredential = @{
        Type = "X509CertAndPassword"
        Usage = "Sign"
        Key = [System.Text.Encoding]::ASCII.GetBytes("MIIDYDCCAki...")
    }
    PasswordCredential = @{
        SecretText = "MKTr0w1..."
    }
    Proof = "eyJ0eXAiOiJ..."
}

Add-MgApplicationKey -ApplicationId $applicationId -BodyParameter $params

```