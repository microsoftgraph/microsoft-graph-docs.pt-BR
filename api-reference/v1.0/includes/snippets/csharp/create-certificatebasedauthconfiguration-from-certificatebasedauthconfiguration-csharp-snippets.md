---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 94315fcd479b1f7634d4b0c517fb76793faaca0f03cae37724066028d61bdcb1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275355"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var certificateBasedAuthConfiguration = new CertificateBasedAuthConfiguration
{
    CertificateAuthorities = new List<CertificateAuthority>()
    {
        new CertificateAuthority
        {
            IsRootAuthority = true,
            Certificate = Encoding.ASCII.GetBytes("Binary")
        }
    }
};

await graphClient.Organization["{organization-id}"].CertificateBasedAuthConfiguration.References
    .Request()
    .AddAsync(certificateBasedAuthConfiguration);

```