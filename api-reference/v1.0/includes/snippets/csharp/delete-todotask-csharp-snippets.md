---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c2a448e03b40faedd27d6bb0131bcd7220c739b2
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904929"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Todo.Lists["AAMkADA1MTHgwAAA="].Tasks["721a35e2-35e2-721a-e235-1a72e2351a72"]
    .Request()
    .DeleteAsync();

```