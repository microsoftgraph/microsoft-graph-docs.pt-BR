---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 184c2a6a98431d7e7221a65e9a04187dc3f6f7c3
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338431"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Search.Qnas["{search.qna-id}"]
    .Request()
    .DeleteAsync();

```