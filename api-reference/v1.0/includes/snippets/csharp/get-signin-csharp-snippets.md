---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fac5464335631b3293c06618a430bcde5d3a5d11
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783740"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var signIn = await graphClient.AuditLogs.SignIns["{signIn-id}"]
    .Request()
    .GetAsync();

```