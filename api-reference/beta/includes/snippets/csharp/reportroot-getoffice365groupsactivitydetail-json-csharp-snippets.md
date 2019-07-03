---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: baf088394085c2b2186025c3c82ef007a515946b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35477018"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365GroupsActivityDetail = await graphClient.Reports.GetOffice365GroupsActivityDetail('D7')
    .Request()
    .GetAsync();

```