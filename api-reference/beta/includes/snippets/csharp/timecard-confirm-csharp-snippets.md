---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ed346ac100f00e6c78eef8bd9a664263323e5327
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869783"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"].Schedule.TimeCards["{timeCard-id}"]
    .Confirm()
    .Request()
    .PostAsync();

```