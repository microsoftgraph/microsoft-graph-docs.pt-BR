---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d5f0d14d31344865553b29e68f761e7fc8932c39
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2019
ms.locfileid: "36460955"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outcomes = await graphClient.Education.Me.Assignments["{id}"].Submissions["{id}"].Outcomes
    .Request()
    .GetAsync();

```