---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6b0602baa80424c4f4af2fe4aa98670384bb7ac2021d51436283c605ee3fb4de
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327634"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var projectParticipation = new ProjectParticipation
{
    AllowedAudiences = AllowedAudiences.Organization,
    Client = new CompanyDetail
    {
        Department = "Corporate Marketing",
        WebUrl = "https://www.contoso.com"
    }
};

await graphClient.Me.Profile.Projects["{projectParticipation-id}"]
    .Request()
    .UpdateAsync(projectParticipation);

```