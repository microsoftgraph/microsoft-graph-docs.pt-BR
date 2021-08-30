---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 696bf9158f8709962db8b36745f97483e8a12446957f43ebaabe7d7aecf8fe00
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157967"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissionGrants = await graphClient.Teams["{team-id}"].PermissionGrants
    .Request()
    .GetAsync();

```