---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6b9bd055a7a3f654bb73f7fa5bd942fe24145abb
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302201"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reason = RejectReason.Busy;

await graphClient.Communications.Calls["57dab8b1-894c-409a-b240-bd8beae78896"]
    .Reject(reason,null)
    .Request()
    .PostAsync();

```