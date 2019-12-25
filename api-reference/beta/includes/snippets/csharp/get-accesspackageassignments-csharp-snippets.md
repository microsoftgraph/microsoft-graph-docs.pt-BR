---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9a78b4ba25b6ecf949652da74b2e7a14785ee33b
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "37992910"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignments = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignments
    .Request()
    .GetAsync();

```