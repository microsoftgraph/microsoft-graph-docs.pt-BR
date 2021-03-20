---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ca1ad5708bfa15ef2394300bcbc4c34367bbe2f5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943983"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var organizationalBranding = await graphClient.Organization["{organization-id}"].Branding
    .Request()
    .GetAsync();

```