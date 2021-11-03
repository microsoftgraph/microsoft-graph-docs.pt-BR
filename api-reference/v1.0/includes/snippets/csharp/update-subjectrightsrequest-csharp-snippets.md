---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b1ad790e2e58b58e394bc530b81cfb0d9d0dc7b4
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687867"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subjectRightsRequest = new SubjectRightsRequestObject
{
    InternalDueDateTime = DateTimeOffset.Parse("2021-08-30T00:00:00Z")
};

await graphClient.Privacy.SubjectRightsRequests["{subjectRightsRequest-id}"]
    .Request()
    .UpdateAsync(subjectRightsRequest);

```