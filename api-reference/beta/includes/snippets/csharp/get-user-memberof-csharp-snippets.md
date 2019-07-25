---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b4b0dc4cc0c2aeaa733c0b5f7f0429527261ace0
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35707098"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var memberOf = await graphClient.Me.MemberOf
    .Request()
    .GetAsync();

```