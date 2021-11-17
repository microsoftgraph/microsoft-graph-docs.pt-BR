---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b8e70bddc459580d920363022eed3e4075ee5b3151f00835028af8b23b94581e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159717"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var callbackUri = "callbackUri-value";

var mediaConfig = new AppHostedMediaConfig
{
    Blob = "<Media Session Configuration Blob>"
};

var acceptedModalities = new List<Modality>()
{
    Modality.Audio
};

var participantCapacity = 200;

await graphClient.Communications.Calls["{call-id}"]
    .Answer(callbackUri,mediaConfig,acceptedModalities,participantCapacity)
    .Request()
    .PostAsync();

```