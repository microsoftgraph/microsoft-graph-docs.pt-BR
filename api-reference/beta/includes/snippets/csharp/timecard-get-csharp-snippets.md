---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ab1a33b2805daaa480397a1c9334f43035898b62
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869509"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var timeCard = await graphClient.Teams["{team-id}"].Schedule.TimeCards["{timeCard-id}"]
    .Request()
    .GetAsync();

```