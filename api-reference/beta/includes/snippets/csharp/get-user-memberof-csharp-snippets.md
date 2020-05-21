---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ec29c69ad56e51eec38dbeaa247e65bbf56f177d
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336465"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var memberOf = await graphClient.Users["{id}"].MemberOf
    .Request()
    .GetAsync();

```