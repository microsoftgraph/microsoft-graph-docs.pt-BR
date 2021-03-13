---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b41519e4077945d56d70c57b9be38477e9959918
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777521"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printServiceEndpoint = await graphClient.Print.Services["{printService-id}"].Endpoints["{printServiceEndpoint-id}"]
    .Request()
    .GetAsync();

```