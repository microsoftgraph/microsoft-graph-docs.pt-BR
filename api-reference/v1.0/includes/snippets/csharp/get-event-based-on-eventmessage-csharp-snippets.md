---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 626404feabb33c582058035a5615d0eef34960384806c2f94de57718ee07ea99
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57407109"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = await graphClient.Me.Messages["{message-id}"]
    .Request()
    .Expand("eventMessage/event")
    .GetAsync();

```