---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 52edce7be4867baa2710b6d69a7cf3fa44b21a9a
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614808"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var domains = await graphClient.Domains
    .Request()
    .GetAsync();

```