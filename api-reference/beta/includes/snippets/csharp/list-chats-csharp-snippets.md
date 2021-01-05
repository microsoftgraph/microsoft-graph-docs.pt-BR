---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 337d5a49a252a095f6cb37f55f36ce19135df283
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49752899"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chats = await graphClient.Users["8b081ef6-4792-4def-b2c9-c363a1bf41d5"].Chats
    .Request()
    .GetAsync();

```