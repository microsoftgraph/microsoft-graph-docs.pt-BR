---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 58f1d573dfad1773491203212619cf76cb88f2b0
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015444"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schools = await graphClient.Education.Classes["{class-id}"].Schools
    .Request()
    .GetAsync();

```