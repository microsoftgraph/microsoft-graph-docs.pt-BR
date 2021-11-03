---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 54a4d2235e1686beea958e002a734a29b9d29267
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687902"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var notes = await graphClient.Privacy.SubjectRightsRequests["{subjectRightsRequest-id}"].Notes
    .Request()
    .GetAsync();

```