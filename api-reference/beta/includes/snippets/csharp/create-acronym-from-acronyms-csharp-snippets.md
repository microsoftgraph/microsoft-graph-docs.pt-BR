---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 55b269032031b287a4b633613e4ab02ee576c116
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338072"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var acronym = new Microsoft.Graph.Search.Acronym
{
    DisplayName = "DNN",
    StandsFor = "Deep Neural Network",
    Description = "A deep neural network is a neural network with a certain level of complexity, a neural network with more than two layers.",
    WebUrl = "http://microsoft.com/deep-neural-network",
    State = Microsoft.Graph.Search.AnswerState.Draft
};

await graphClient.Search.Acronyms
    .Request()
    .AddAsync(acronym);

```