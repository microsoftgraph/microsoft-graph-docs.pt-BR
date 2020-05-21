---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3f91ded0a9725ea1146ef6208619dc1bdbd99fda
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333345"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignments = await graphClient.Users["{id}"].AppRoleAssignments
    .Request()
    .GetAsync();

```