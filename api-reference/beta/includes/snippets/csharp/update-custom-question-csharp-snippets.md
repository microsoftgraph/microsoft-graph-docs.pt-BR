---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8b7d2ab89452b9681d461782ef6d624ad69fce9f
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60558591"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var meetingRegistrationQuestion = new MeetingRegistrationQuestion
{
    AnswerInputType = AnswerInputType.RadioButton,
    AnswerOptions = new List<String>()
    {
        "Software Engineer",
        "Software Development Manager",
        "Product Manager",
        "Data scientist",
        "Other"
    }
};

await graphClient.Me.OnlineMeetings["{onlineMeeting-id}"].Registration.CustomQuestions["{meetingRegistrationQuestion-id}"]
    .Request()
    .UpdateAsync(meetingRegistrationQuestion);

```