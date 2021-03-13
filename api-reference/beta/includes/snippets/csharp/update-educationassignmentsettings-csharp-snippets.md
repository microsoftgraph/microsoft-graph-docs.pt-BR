---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d77885c59d5696773c8299c406f6545368377292
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786642"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationAssignmentSettings = new EducationAssignmentSettings
{
    SubmissionAnimationDisabled = true
};

await graphClient.Education.Classes["{educationClass-id}"].AssignmentSettings
    .Request()
    .UpdateAsync(educationAssignmentSettings);

```