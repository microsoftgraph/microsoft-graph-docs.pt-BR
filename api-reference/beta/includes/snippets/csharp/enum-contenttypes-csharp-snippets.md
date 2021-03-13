---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 73cb1f26099fc4cda9e2ee1fcd065956fa0f4052
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770489"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contentTypes = await graphClient.Sites["{site-id}"].ContentTypes
    .Request()
    .GetAsync();

```