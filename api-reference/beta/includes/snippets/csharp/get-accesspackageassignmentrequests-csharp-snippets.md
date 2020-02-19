---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a5455fa3ae11ff13225223a8dd6e796dcf261e55
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "37992917"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignmentRequests = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentRequests
    .Request()
    .GetAsync();

```