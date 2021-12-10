---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b4f9f3bab746487c1aa03ec532da2b4ac01ce3be
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687570"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Privacy.SubjectRightsRequests["{subjectRightsRequest-id}"]
    .GetFinalReport()
    .Request()
    .GetAsync();

```