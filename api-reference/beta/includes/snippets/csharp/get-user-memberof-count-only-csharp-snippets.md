---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3dd37bfe6667ef4180b565901f051ee9ec171e2d
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336469"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var int32 = await graphClient.Users["{id}"].MemberOf.$count
    .Request()
    .Header("ConsistencyLevel","eventual")
    .GetAsync();

```