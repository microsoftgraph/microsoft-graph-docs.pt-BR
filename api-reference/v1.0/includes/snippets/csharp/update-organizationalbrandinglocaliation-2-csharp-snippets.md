---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d92c1914a0e4675647a2ca5a957265251736dcde
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62126144"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = new System.IO.MemoryStream(Encoding.UTF8.GetBytes(@"<Image>
"));

var branding = new OrganizationalBranding();
branding.BannerLogo = stream;

await graphClient.Organization["{organization-id}"].Branding
    .Request()
    .UpdateAsync(branding);

```