---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fa5919022ec01dda8d0a961d2313bad25b963097
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941573"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var openShiftChangeRequests = await graphClient.Teams["{team-id}"].Schedule.OpenShiftChangeRequests
    .Request()
    .GetAsync();

```