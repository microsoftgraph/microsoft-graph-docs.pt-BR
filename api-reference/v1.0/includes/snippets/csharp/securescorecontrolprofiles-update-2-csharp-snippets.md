---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c0725a58fbd28f90ac4679c63e14d1658fdb2475
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948749"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var secureScoreControlProfile = new SecureScoreControlProfile
{
    VendorInformation = new SecurityVendorInformation
    {
        Provider = "SecureScore",
        ProviderVersion = null,
        SubProvider = null,
        Vendor = "Microsoft"
    },
    AdditionalData = new Dictionary<string, object>()
    {
        {"assignedTo", ""},
        {"comment", "control is reviewed"},
        {"state", "Reviewed"}
    }
};

await graphClient.Security.SecureScoreControlProfiles["{secureScoreControlProfile-id}"]
    .Request()
    .UpdateAsync(secureScoreControlProfile);

```