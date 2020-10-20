---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a0cce39cc24a98e3c0a19968d1d8f0b40292a6c6
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605967"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var createdObjects = await graphClient.Me.CreatedObjects
    .Request()
    .GetAsync();

```