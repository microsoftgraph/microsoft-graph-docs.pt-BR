---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0985e3ec9e2423832a657ccb3f8bbd6874412093
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220249"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var signIns = await graphClient.AuditLogs.SignIns
    .Request()
    .Filter("startsWith(appDisplayName,'Graph')")
    .Top(10)
    .GetAsync();

```