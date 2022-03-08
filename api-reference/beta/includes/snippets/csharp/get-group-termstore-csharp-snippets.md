---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3aa164cb72d74fcd59b48824be23b8d847f9c1ff
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337093"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = await graphClient.Sites["{site-id}"].TermStore.Groups["{termStore.group-id}"]
    .Request()
    .GetAsync();

```