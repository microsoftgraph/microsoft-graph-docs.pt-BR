---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 939ea488efae8651a86ff8610d16820f242cc4fa
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873288"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365GroupsActivityGroupCounts = await graphClient.Reports
    .GetOffice365GroupsActivityGroupCounts('D7')
    .Request()
    .GetAsync();

```