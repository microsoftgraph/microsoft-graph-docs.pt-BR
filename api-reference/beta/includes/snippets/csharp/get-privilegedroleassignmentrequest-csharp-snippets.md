---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1bbf2bec69840573c7b0642fa28273883b723c4e
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616861"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoleAssignmentRequests = await graphClient.PrivilegedRoleAssignmentRequests
    .Request()
    .GetAsync();

```