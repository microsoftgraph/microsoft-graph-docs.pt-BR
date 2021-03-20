---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4a7517a3137de6bad89d97faa4b83595e35da79f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953474"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var openShifts = await graphClient.Teams["{team-id}"].Schedule.OpenShifts
    .Request()
    .GetAsync();

```