---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5ef61d8020fa190a0b238b6f7cdc5abdb7cee8272d9318a6fde57c2d98d0ed76
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327305"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedApproval = new PrivilegedApproval
{
    ApprovalState = ApprovalState.Pending,
    ApproverReason = "approverReason-value"
};

await graphClient.PrivilegedApproval["{privilegedApproval-id}"]
    .Request()
    .UpdateAsync(privilegedApproval);

```