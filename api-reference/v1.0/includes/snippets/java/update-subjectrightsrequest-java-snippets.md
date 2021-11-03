---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 919287056f2de02c3fe4ee32b0111dced5c9f505
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687863"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SubjectRightsRequest subjectRightsRequest = new SubjectRightsRequest();
subjectRightsRequest.internalDueDateTime = OffsetDateTimeSerializer.deserialize("2021-08-30T00:00:00Z");

graphClient.privacy().subjectRightsRequests("{subjectRightsRequestId}")
    .buildRequest()
    .patch(subjectRightsRequest);

```