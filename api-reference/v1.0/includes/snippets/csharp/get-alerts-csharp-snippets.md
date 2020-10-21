---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7bf07cb98320e2f06b14a844161a67289bb8ffff
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604823"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var alerts = await graphClient.Security.Alerts
    .Request()
    .GetAsync();

```