---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 38a64487b2df8baf60e99472c53aaa44404d97b0
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996097"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Submissions["{educationSubmission-id}"]
    .Reassign()
    .Request()
    .Header("Prefer","include-unknown-enum-members")
    .PostAsync();

```