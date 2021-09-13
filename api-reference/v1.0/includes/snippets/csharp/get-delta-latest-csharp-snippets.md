---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3f494a038ac5efa8958b9e1d2815ce74a9b83e9415fa369dfa55799a1be1fc29
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100273"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("token", "latest")
};

var delta = await graphClient.Me.Drive.Root
    .Delta()
    .Request( queryOptions )
    .GetAsync();

```