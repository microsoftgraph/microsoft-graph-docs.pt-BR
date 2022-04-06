---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a4fd65f86c6d12afb6b8fc4520fe7e94efb25987
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757763"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var signIns = await graphClient.AuditLogs.SignIns
    .Request()
    .Filter("(signInEventTypes/any(t: t ne 'interactiveUser'))")
    .OrderBy("createdDateTime DESC")
    .Top(10)
    .GetAsync();

```