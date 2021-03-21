---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7592ff5f6b5d7d462287a673457e3f38767895bb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954388"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var openShiftChangeRequest = await graphClient.Teams["{team-id}"].Schedule.OpenShiftChangeRequests["{openShiftChangeRequest-id}"]
    .Request()
    .GetAsync();

```