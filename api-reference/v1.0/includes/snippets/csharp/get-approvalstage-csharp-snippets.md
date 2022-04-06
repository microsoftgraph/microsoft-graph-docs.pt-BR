---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3e046f298d26e86da938c9f5544b8a6ef0a0b82a
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516398"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var approvalStage = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentApprovals["{approval-id}"].Stages["{approvalStage-id}"]
    .Request()
    .GetAsync();

```