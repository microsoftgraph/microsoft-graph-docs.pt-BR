---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b7f45bf7aedd0f67c1437532f388475d8d4445518e9f070d1e2a624634ba8681
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216626"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var owners = await graphClient.ServicePrincipals["{servicePrincipal-id}"].Owners
    .Request()
    .GetAsync();

```