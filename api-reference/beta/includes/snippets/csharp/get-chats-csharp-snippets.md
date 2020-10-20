---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e5abc9ccd9e4790bcaa7b5dda3fdadc3d114ac0a
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614969"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chats = await graphClient.Users["{id}"].Chats
    .Request()
    .GetAsync();

```