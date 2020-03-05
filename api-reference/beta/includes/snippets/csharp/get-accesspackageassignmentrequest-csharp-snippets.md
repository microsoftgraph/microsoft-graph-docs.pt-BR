---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 71408a800e78ceae5544f7a2186617d41dae7667
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "37992855"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignmentRequest = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentRequests["{id}"]
    .Request()
    .GetAsync();

```