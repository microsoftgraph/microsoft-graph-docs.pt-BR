---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 92e9725708d7be698bff3e44ff7f49b2638228fe
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871476"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getYammerActivityUserCounts = await graphClient.Reports
    .GetYammerActivityUserCounts('D7')
    .Request()
    .GetAsync();

```