---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 85e58fb14ffbf76253320cf0ffe271f8433b7d6c
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63351130"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("$count", "true")
};

var devices = await graphClient.Devices
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Search("displayName:Android")
    .GetAsync();

```