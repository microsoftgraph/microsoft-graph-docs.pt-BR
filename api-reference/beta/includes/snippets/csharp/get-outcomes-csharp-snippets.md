---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 86017afa398f7e3395245f00cd36133f661785a5
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52254191"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outcomes = await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Submissions["{educationSubmission-id}"].Outcomes
    .Request()
    .GetAsync();

```