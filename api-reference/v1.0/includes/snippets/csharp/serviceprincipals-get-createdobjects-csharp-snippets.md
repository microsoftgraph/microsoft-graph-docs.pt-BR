---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 99e198b94e9018f1c88f913ef068dfc7a5678c3a
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336049"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var createdObjects = await graphClient.ServicePrincipals["{id}"].CreatedObjects
    .Request()
    .GetAsync();

```