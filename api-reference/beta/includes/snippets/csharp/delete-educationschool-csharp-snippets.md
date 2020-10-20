---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0933b3bcf9bdabc4026ba9a9c4c05d530e799dda
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606187"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Schools["10002"]
    .Request()
    .DeleteAsync();

```