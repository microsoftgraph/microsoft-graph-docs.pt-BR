---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 66c3623159482be354d510d4102fc3cce910d3b0
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333114"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var keyCredential = new KeyCredential
{
    Type = "X509CertAndPassword",
    Usage = "Sign",
    Key = "MIIDYDCCAki..."
};

var passwordCredential = new PasswordCredential
{
    SecretText = "MKTr0w1..."
};

var proof = "eyJ0eXAiOiJ...";

await graphClient.Applications["{id}"]
    .AddKey(keyCredential,proof,passwordCredential)
    .Request()
    .PostAsync();

```