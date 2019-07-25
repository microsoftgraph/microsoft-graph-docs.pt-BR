---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fa379249be953292241333f23e5667b12333ce8f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875558"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var my = await graphClient.PrivilegedRoleAssignmentRequests
    .My()
    .Request()
    .GetAsync();

```