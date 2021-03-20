---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: af322bca1c0486b0f9fbcfdbec1251427ade10dc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50949288"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var organizationalBrandingLocalization = new OrganizationalBrandingLocalization
{
    BackgroundColor = "#00000F",
    Id = "fr"
};

await graphClient.Organization["{organization-id}"].Branding.Localizations
    .Request()
    .AddAsync(organizationalBrandingLocalization);

```