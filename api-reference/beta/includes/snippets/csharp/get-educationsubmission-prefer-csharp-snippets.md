---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b29e1132b39c748af234a1c30c5403dc4cbb40b4
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61524915"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSubmission = await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Submissions["{educationSubmission-id}"]
    .Request()
    .Header("Prefer","include-unknown-enum-members")
    .GetAsync();

```