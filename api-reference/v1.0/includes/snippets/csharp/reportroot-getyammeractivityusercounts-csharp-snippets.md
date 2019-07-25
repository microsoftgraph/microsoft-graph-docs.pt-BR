---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 24f4b75a3ce7d4ffdda3f1415af6bf5df65b3da0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891434"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetYammerActivityUserCounts('D7')
    .Request()
    .GetAsync();

```