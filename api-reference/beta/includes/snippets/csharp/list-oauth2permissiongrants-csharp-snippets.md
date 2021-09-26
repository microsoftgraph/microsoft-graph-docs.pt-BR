---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e99ed3448a9e0103090b8081d73ccbd96a92526d512e46825b0e9ae855d0acfc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156468"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var oauth2PermissionGrants = await graphClient.Oauth2PermissionGrants
    .Request()
    .GetAsync();

```