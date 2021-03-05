---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f3f7521ae3c1aaf56baae7b22d7bffc197de75e0
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470310"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationAssignmentDefaults = new EducationAssignmentDefaults
{
    AddedStudentAction = EducationAddedStudentAction.AssignIfOpen,
    NotificationChannelUrl = "https://graph.microsoft.com/beta/teams('id')/channels('id')"
};

await graphClient.Education.Classes["{id}"].AssignmentDefaults
    .Request()
    .UpdateAsync(educationAssignmentDefaults);

```