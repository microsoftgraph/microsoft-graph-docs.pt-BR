---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: afbc0d8b69a2f7c20feac7538130db4512f5fa05
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333267"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var int32 = await graphClient.Groups["{id}"].TransitiveMembers.$count
    .Request()
    .Header("ConsistencyLevel","eventual")
    .GetAsync();

```