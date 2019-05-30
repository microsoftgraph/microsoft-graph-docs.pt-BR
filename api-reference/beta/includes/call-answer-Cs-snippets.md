---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6a27aa30b8d48cd6a7c79bbcf4224440dcdd15b2
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "34546557"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var callbackUri = "callbackUri-value";

var mediaConfig = new MediaConfig
{
    Blob = "<media config blob>"
};

var acceptedModalities = new List<String>()
{
    "audio"
};

await graphClient.App.Calls["{id}"]
    .Answer(callbackUri,mediaConfig,acceptedModalities)
    .Request()
    .PostAsync();

```