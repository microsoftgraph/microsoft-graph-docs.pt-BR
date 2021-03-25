---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e048d7c823d6f2965595edd57c16f34f64fcc8f7
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51211135"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Messages
    .Delta()
    .Request()
    .GetAsync();

```