---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 50e11e49e6fc9b77949ec6b3f0dc814140623b79
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561826"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authoredNote = new AuthoredNote
{
    Content = new ItemBody
    {
        Content = "String",
        ContentType = BodyType.Text
    }
};

await graphClient.Privacy.SubjectRightsRequests["{subjectRightsRequest-id}"].Notes
    .Request()
    .AddAsync(authoredNote);

```