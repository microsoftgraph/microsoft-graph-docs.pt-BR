---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2010393211ece3e62ba0cea36b8be3ffdb8774c0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792878"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("format", "{format}")
};

var stream = await graphClient.Drive.Items["{driveItem-id}"].Content
    .Request( queryOptions )
    .GetAsync();

```