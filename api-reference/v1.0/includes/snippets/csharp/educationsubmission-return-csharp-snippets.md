---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 919ab665a2ff2917c8dc8dfac7c27b487a0b5baa
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993368"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Submissions["{educationSubmission-id}"]
    .Return()
    .Request()
    .PostAsync();

```