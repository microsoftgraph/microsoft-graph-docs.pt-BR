---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: afc0f6c62f9c639c5fad8cbc2986e5f57c59aac6
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605502"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Chats["{id}"].Messages
    .Request()
    .GetAsync();

```