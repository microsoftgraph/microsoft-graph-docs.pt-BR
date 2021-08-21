---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b53f99555d02a03124680955396b6b5f46cca0d5324f9a947d4572f0b7b99326
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215125"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoleAssignmentRequests = await graphClient.PrivilegedRoleAssignmentRequests
    .Request()
    .GetAsync();

```