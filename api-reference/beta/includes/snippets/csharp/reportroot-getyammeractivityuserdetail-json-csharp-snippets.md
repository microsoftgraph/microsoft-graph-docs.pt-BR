---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 18b2c35c2e44f3172172be1db4c52bd012fd810a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871537"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getYammerActivityUserDetail = await graphClient.Reports
    .GetYammerActivityUserDetail('D7')
    .Request()
    .GetAsync();

```