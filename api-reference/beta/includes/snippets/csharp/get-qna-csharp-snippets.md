---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1f522fe1a4e1fe615ff0ccdc48b1ae83d6ec168d
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338012"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var qna = await graphClient.Search.Qnas["{search.qna-id}"]
    .Request()
    .GetAsync();

```