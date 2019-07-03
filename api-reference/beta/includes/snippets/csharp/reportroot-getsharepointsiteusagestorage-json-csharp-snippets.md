---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2691ba68bb732e0443284b1b222975e24752eef8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35517639"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSharePointSiteUsageStorage = await graphClient.Reports.GetSharePointSiteUsageStorage('D7')
    .Request()
    .GetAsync();

```