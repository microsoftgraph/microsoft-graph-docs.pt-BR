---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a6d695c7d6c77ffdf70761d2c57e1c5dd9a9b810
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536656"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reason = RejectReason.None;

await graphClient.App.Calls["{id}"]
    .Reject(reason)
    .Request()
    .PostAsync();

```