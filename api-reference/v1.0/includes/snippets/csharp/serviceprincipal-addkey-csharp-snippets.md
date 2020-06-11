---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9e3990170ece86346b8b26ef1a971cd11f1f6eb8
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44683700"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var keyCredential = new KeyCredential
{
    Type = "X509CertAndPassword",
    Usage = "Sign",
    Key = Encoding.ASCII.GetBytes("MIIDYDCCAki...")
};

var passwordCredential = new PasswordCredential
{
    SecretText = "MKTr0w1..."
};

var proof = "eyJ0eXAiOiJ...";

await graphClient.Serviceprincipals["{id}"]
    .AddKey(keyCredential,proof,passwordCredential)
    .Request()
    .PostAsync();

```