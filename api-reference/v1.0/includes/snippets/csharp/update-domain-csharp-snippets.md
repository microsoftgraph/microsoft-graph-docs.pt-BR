---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 50954e9f2abbb5fee3a3f947f16bc894bb9c4cfb
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606521"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var domain = new Domain
{
    IsDefault = true,
    SupportedServices = new List<String>()
    {
        "Email",
        "OfficeCommunicationsOnline"
    }
};

await graphClient.Domains["contoso.com"]
    .Request()
    .UpdateAsync(domain);

```