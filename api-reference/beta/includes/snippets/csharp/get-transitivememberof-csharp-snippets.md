---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cd75b41a552511ea1c0a35464626e2e9e500b144
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336726"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var transitiveMemberOf = await graphClient.Users["{id}"].TransitiveMemberOf
    .Request()
    .GetAsync();

```