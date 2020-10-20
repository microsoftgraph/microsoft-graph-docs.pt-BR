---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ef6caa3f9a541be3e7e525818b5079343c77bf26
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620253"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversation = await graphClient.Groups["{id}"].Conversations["{id}"]
    .Request()
    .GetAsync();

```