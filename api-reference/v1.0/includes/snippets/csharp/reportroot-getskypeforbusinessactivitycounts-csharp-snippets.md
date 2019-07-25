---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ef422be4b208fc9800178f457809ec6e22bdfc91
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885911"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSkypeForBusinessActivityCounts('D7')
    .Request()
    .GetAsync();

```