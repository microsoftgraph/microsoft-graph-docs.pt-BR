---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2b63b0cfab05fe705a7d996c96efbeeb627b0d61
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62346638"
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

Add-MgServicePrincipalKey -ServicePrincipalId $servicePrincipalId -BodyParameter $params

```