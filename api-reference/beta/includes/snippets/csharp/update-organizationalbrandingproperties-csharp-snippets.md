---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e003c1a771db709397ce0a4a04201d6a2d0f7a91
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523943"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var organizationalBrandingLocalization = new OrganizationalBrandingLocalization
{
    BackgroundColor = "#00000F",
    SignInPageText = "fr"
};

await graphClient.Organization["d69179bf-f4a4-41a9-a9de-249c0f2efb1d"].Branding.Localizations["fr"]
    .Request()
    .PutAsync(organizationalBrandingLocalization);

```