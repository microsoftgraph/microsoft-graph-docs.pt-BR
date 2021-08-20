---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4f61e8c793da409b00da31e82ff0be8ff94522968ffa1c699e3bd1c9a9979546
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326851"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var submittedResources = await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Submissions["{educationSubmission-id}"].SubmittedResources
    .Request()
    .GetAsync();

```