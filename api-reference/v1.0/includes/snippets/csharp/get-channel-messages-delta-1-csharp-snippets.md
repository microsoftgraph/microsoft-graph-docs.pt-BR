---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: db6c345dcec2568057590959de2c00b3bc93e947
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209285"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Messages
    .Delta()
    .Request()
    .Top(2)
    .GetAsync();

```