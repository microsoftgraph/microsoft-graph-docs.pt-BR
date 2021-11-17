---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 34e262a067f11aae398fa5718cfff38b22c758797c7d7a1eda1a952f82ef3ebb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326640"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var callbackUri = "https://bot.contoso.com/api/calls";

var acceptedModalities = new List<Modality>()
{
    Modality.Audio
};

var mediaConfig = new AppHostedMediaConfig
{
    Blob = "<Media Session Configuration Blob>"
};

await graphClient.Communications.Calls["{call-id}"]
    .Answer(callbackUri,mediaConfig,acceptedModalities,null)
    .Request()
    .PostAsync();

```