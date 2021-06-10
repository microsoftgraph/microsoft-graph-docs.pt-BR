---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 40b0cf296bbfe40bc5bde46b2ed527b5b52bc416
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869001"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleAssignments = await graphClient.RoleManagement.CloudPC.RoleAssignments
    .Request()
    .GetAsync();

```