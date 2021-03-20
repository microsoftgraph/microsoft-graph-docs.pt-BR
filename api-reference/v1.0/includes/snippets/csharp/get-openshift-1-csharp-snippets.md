---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e673eaed9cf4765d9b5f276c2e8446083ca06b07
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953509"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var openShift = await graphClient.Teams["{team-id}"].Schedule.OpenShifts["{openShift-id}"]
    .Request()
    .GetAsync();

```