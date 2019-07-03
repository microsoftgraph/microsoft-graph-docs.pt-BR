---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5274fe0cd95babdb2907ce5ae087161e37d6b260
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35476773"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessDeviceUsageUserCounts = await graphClient.Reports.GetSkypeForBusinessDeviceUsageUserCounts('D7')
    .Request()
    .GetAsync();

```