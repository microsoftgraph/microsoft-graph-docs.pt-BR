---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6da78a6366f5337ff0b348d141c1c506dcae6f5b
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48610910"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["11021"].Assignments["19002"].Resources["22002"]
    .Request()
    .DeleteAsync();

```