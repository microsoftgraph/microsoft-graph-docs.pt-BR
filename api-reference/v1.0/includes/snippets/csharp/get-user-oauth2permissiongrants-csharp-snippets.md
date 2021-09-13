---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7141d18df2a2155ef887e76221171d85b317b26b3e958eadcc269df666d920e1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216431"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var oauth2PermissionGrants = await graphClient.Users["{user-id}"].Oauth2PermissionGrants
    .Request()
    .GetAsync();

```