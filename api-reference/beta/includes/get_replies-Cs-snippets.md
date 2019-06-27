---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8525273f3ec881b6b1e3003819ed5894c9bd589c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35329327"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var replies = await graphClient.Chats["{id}"].Messages["{id}"].Replies
    .Request()
    .GetAsync();

```