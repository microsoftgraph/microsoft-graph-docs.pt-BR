---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9e06ecc5ff49aa697d377db19c09d15725093e2e9db47017d2c3d23178173864
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156889"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleAssignmentScheduleRequests = await graphClient.RoleManagement.Directory.RoleAssignmentScheduleRequests
    .Request()
    .GetAsync();

```