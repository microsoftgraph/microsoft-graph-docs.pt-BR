---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7b8464b3c30fa756ae15afa73105b517f3b05d38
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606063"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = await graphClient.Me.Messages["AAMkADYAAAImV_lAAA="]
    .Request()
    .GetAsync();

```