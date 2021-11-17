---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 885074fc052b52b369adff8c582ebd91210bba98eb9183f84fa53a3c3bf90661
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898261"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageResourceRequests = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageResourceRequests
    .Request()
    .GetAsync();

```