---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f3d2d87bb866e31946c2486ea8074b7e0a1d6482
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48603777"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Contacts["{id}"]
    .Request()
    .DeleteAsync();

```