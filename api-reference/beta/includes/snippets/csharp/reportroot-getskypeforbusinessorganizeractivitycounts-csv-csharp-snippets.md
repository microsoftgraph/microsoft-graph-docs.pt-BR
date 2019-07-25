---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dc9a13e5669c01186896fdf19fad951ef17d6e80
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872289"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessOrganizerActivityCounts = await graphClient.Reports
    .GetSkypeForBusinessOrganizerActivityCounts('D7')
    .Request()
    .GetAsync();

```