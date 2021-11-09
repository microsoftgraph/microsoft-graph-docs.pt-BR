---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1581aa84c648eacff7167fa7d8bd58b9b39687c9
ms.sourcegitcommit: ddeee0eec277df06d9e635e5b5c257d14c856273
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2021
ms.locfileid: "60780778"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getApplicableContentTypesForList = await graphClient.Sites["{site-id}"]
    .GetApplicableContentTypesForList("{list-id}")
    .Request()
    .GetAsync();

```