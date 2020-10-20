---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fb345d8ac1c25ff29197cb7646da7af78261c627
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48610442"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directReports = await graphClient.Me.DirectReports
    .Request()
    .GetAsync();

```