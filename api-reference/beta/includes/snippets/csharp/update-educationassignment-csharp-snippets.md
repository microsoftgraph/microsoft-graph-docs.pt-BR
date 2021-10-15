---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2024e85ead2f3b9ff6a7ebfeeeedf4b2aecc44d9
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2021
ms.locfileid: "60365778"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationAssignment = new EducationAssignment
{
    DisplayName = "Reading and review test 09.03 #5",
    Instructions = new EducationItemBody
    {
        ContentType = BodyType.Text,
        Content = "Read chapter 5 and write your review"
    },
    DueDateTime = DateTimeOffset.Parse("2021-09-10T00:00:00Z"),
    AddedStudentAction = EducationAddedStudentAction.None,
    AddToCalendarAction = EducationAddToCalendarOptions.StudentsAndPublisher
};

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"]
    .Request()
    .UpdateAsync(educationAssignment);

```