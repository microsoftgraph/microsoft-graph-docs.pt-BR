---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 920680f944ec135def951fd59dea8e0a530b73a0
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015572"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contract = await graphClient.Contracts["{id}"]
    .Request()
    .GetAsync();

```