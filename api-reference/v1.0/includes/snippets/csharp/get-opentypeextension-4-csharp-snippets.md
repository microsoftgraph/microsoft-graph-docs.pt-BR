---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5469d7154ea22bc1e23bdac08988d39de66d9f0b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809714"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var extension = await graphClient.Groups["{group-id}"].Threads["{conversationThread-id}"].Posts["{post-id}"].Extensions["{extension-id}"]
    .Request()
    .GetAsync();

```