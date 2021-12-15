---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a4742e440591a19d11a6fb62cea53a1af9aa2948
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525842"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var submissions = await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Submissions
    .Request()
    .Header("Prefer","include-unknown-enum-members")
    .GetAsync();

```