---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 23e517a494ba51471e676c95969cfcbcc77042e0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327114"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetOffice365ActiveUserCounts("D7")
    .Request()
    .GetAsync();

```