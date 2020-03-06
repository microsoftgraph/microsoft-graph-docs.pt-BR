---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a283d07e7c665b13a15d092579b75984126f9e93
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638652"
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
            Certificate = "Binary"
        }
    }
};

await graphClient.Organization["{id}"].CertificateBasedAuthConfiguration
    .Request()
    .AddAsync(certificateBasedAuthConfiguration);

```