---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ab0d1236f8704f312086df48451479144799a454
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687491"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subjectRightsRequests = await graphClient.Privacy.SubjectRightsRequests
    .Request()
    .GetAsync();

```