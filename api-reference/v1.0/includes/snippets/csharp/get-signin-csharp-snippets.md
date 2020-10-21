---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aa1f4d787169e5f37340ca755e6f0f75dc34d61f
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48603584"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var signIn = await graphClient.AuditLogs.SignIns["{id}"]
    .Request()
    .GetAsync();

```