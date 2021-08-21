---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c6cd04366b089381c622ec852c2f5c9278ef68ff55aad78432250683b8b24759
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273269"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.PrivilegedRoleAssignmentRequests["{privilegedRoleAssignmentRequest-id}"]
    .Cancel()
    .Request()
    .PostAsync();

```