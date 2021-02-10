---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7e56a2ace3c094f6b6c072be4f2c258b806058a1
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50179458"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var organizationalBranding = new OrganizationalBranding
{
    BackgroundColor = "#FFFF33"
};

await graphClient.Organization["d69179bf-f4a4-41a9-a9de-249c0f2efb1d"].Branding
    .Request()
    .PutAsync(organizationalBranding);

```