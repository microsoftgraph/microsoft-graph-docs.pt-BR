---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a446c19fcbcf6ea95976171668cf06129ed32069
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884651"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetOffice365GroupsActivityFileCounts('D7')
    .Request()
    .GetAsync();

```