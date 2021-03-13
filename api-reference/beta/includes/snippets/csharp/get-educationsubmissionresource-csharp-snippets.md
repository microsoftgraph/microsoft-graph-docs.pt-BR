---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d6f466fecf3eaa32689a16913eebd97fe62453d8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786130"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationSubmissionResource = await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Submissions["{educationSubmission-id}"].Resources["{educationSubmissionResource-id}"]
    .Request()
    .GetAsync();

```