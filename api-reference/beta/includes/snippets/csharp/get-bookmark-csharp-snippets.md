---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d0873c3925f5e31731c1b9518b60152d7d5c1c9a
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338052"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookmark = await graphClient.Search.Bookmarks["{search.bookmark-id}"]
    .Request()
    .GetAsync();

```