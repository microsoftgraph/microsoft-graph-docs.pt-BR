---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ae19d40b04ce0ff59f23e30bc765801ada7cc21d3a1c84802b036849f25365c3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103122"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationThread = await graphClient.Groups["{group-id}"].Threads["{conversationThread-id}"]
    .Request()
    .GetAsync();

```