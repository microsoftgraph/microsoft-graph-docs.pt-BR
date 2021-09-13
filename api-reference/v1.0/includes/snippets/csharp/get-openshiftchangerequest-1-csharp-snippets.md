---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 83a13c7d57444ba259da6ad76caf2592f5945dfeb4c4badc7c2843a2f87fc727
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327901"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var openShiftChangeRequest = await graphClient.Teams["{team-id}"].Schedule.OpenShiftChangeRequests["{openShiftChangeRequest-id}"]
    .Request()
    .GetAsync();

```