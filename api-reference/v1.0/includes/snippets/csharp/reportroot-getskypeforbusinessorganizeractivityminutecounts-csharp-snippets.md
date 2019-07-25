---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fa94caa8e814bc96043d4edbad4a8b74dc2b3d31
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892346"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSkypeForBusinessOrganizerActivityMinuteCounts('D7')
    .Request()
    .GetAsync();

```