---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: da3c1e4eea7489683601e295f66df54c22be57f6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872408"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessActivityUserCounts = await graphClient.Reports
    .GetSkypeForBusinessActivityUserCounts('D7')
    .Request()
    .GetAsync();

```