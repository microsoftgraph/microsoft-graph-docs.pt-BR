---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fec583e1a20ea871760fd812511f1714556f1a8d
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905007"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessage = await graphClient.Teams["{id}"].Channels["{id}"].Messages["delta"]
    .Request()
    .Top(2)
    .GetAsync();

```