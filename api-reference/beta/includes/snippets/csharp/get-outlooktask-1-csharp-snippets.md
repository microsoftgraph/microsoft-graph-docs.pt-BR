---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 76aa7f4f4b57c62c7b7072eb9588f9b2cf256b82
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957596"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookTask = await graphClient.Me.Outlook.Tasks["{outlookTask-id}"]
    .Request()
    .GetAsync();

```