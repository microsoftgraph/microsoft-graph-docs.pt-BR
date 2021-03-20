---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ec9f3965d13e6c24503c67cdc8853fb19b6fac76
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955748"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Organization["{organization-id}"].Branding
    .Request()
    .DeleteAsync();

```