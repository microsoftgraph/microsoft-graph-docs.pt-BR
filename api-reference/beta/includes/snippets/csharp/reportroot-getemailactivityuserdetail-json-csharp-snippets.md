---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d75ea17788c38a44b37139ede0a6363e0115e093
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35519096"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getEmailActivityUserDetail = await graphClient.Reports.GetEmailActivityUserDetail('D7')
    .Request()
    .GetAsync();

```