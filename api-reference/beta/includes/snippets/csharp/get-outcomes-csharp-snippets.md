---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3d6131f204e284ea198c9a742da7294268921f04
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794858"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outcomes = await graphClient.Education.Me.Assignments["{educationAssignment-id}"].Submissions["{educationSubmission-id}"].Outcomes
    .Request()
    .GetAsync();

```