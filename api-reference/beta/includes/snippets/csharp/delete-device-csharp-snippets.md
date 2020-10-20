---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ab8bde42fb4ca337230599efbf7c4da029724608
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616697"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Devices["{id}"]
    .Request()
    .DeleteAsync();

```