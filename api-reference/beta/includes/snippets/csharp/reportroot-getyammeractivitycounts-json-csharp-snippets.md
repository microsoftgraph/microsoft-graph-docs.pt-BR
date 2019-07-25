---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b1876fe9a052fdb51788092ef6d902a222612c71
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871436"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getYammerActivityCounts = await graphClient.Reports
    .GetYammerActivityCounts('D7')
    .Request()
    .GetAsync();

```