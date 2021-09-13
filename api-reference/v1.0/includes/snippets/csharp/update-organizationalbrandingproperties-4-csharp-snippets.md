---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 955a6896ae2954c0dc5a9e40dacaa97c9b1a9e2806129df33bfd32953c625ee6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56897770"
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