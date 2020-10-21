---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ff80ff9b4fb36607e2bf97d3d1c9f8842cbb79d7
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605786"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subscription = await graphClient.Subscriptions["{id}"]
    .Request()
    .GetAsync();

```