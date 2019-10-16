---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7d0f87d621356c71a2daeda99565cabc7ce57b22
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37544110"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var callbackUri = "callbackUri-value";

var mediaConfig = new AppHostedMediaConfig
{
    Blob = "<media config blob>"
};

var acceptedModalities = new List<Modality>()
{
    Modality.Audio
};

await graphClient.App.Calls["{id}"]
    .Answer(callbackUri,mediaConfig,acceptedModalities)
    .Request()
    .PostAsync();

```