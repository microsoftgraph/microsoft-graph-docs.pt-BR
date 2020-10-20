---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3783e4d3f5585c52b5b75b9ba9bc50460476de03
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618268"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["11021"].Assignments["19002"].Submissions["850f51b7"]
    .Return()
    .Request()
    .PostAsync();

```