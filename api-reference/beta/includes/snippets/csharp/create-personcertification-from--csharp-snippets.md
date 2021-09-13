---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9ae8bc7c7126277b2ec9a369b70c15539a2ab542413a7e2d93aa54c2b6629107
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274898"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personCertification = new PersonCertification
{
    CertificationId = "KB-1235466333663322",
    Description = "Blackbelt in Marketing - Brand Management",
    DisplayName = "Marketing Blackbelt - Brand Management",
    ThumbnailUrl = "https://iame.io/dfhdfdfd334.jpg",
    WebUrl = "https://www.iame.io/blackbelt"
};

await graphClient.Me.Profile.Certifications
    .Request()
    .AddAsync(personCertification);

```