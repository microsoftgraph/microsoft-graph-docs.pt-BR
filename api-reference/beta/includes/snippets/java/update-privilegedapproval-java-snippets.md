---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7084bf475ce05cd4411be01a526ce6b87da1c4f61a03131c6f351b4e3e67fcaf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327306"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedApproval privilegedApproval = new PrivilegedApproval();
privilegedApproval.approvalState = ApprovalState.PENDING;
privilegedApproval.approverReason = "approverReason-value";

graphClient.privilegedApproval("{requestId}")
    .buildRequest()
    .patch(privilegedApproval);

```