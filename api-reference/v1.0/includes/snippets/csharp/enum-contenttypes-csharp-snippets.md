---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 73cb1f26099fc4cda9e2ee1fcd065956fa0f4052
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59026051"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contentTypes = await graphClient.Sites["{site-id}"].ContentTypes
    .Request()
    .GetAsync();

```