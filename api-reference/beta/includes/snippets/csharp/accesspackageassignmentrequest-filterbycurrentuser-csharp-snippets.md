---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 67db238aeb820c336056e662732f6e49b6685b37
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52473938"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterByCurrentUser = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackages
    .FilterByCurrentUser(AccessPackageFilterByCurrentUserOptions.AllowedRequestor)
    .Request()
    .GetAsync();

```