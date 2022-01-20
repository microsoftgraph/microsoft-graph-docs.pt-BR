---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 38a64487b2df8baf60e99472c53aaa44404d97b0
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62111178"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Submissions["{educationSubmission-id}"]
    .Reassign()
    .Request()
    .Header("Prefer","include-unknown-enum-members")
    .PostAsync();

```