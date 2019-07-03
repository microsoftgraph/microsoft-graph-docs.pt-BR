---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aa4aa7a6c0df64cd38f1639af9f24078440462f3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492280"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetEmailAppUsageAppsUserCounts('D7')
    .Request()
    .GetAsync();

```