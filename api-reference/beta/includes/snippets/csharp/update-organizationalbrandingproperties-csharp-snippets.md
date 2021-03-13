---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 244a12cae3af765a40b980acada5d3c9254442c0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784999"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var organizationalBranding = new OrganizationalBranding
{
    BackgroundColor = "#FFFF33"
};

await graphClient.Organization["{organization-id}"].Branding
    .Request()
    .PutAsync(organizationalBranding);

```