---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7f564744aef5a15791cc14d91d3c7e596afa3f17
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609211"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contracts = await graphClient.Contracts
    .Request()
    .GetAsync();

```