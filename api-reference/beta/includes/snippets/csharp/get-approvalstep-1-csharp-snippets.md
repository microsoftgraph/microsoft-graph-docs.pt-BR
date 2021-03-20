---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b05793256c80af197c1554f359298c6d8f19dba4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942568"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var steps = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentApprovals["{approval-id}"].Steps
    .Request()
    .GetAsync();

```