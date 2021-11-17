---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e2deb462a3a4696325bd47a5693ccd3472b544e6
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687495"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SubjectRightsRequestCollectionPage subjectRightsRequests = graphClient.privacy().subjectRightsRequests()
    .buildRequest()
    .get();

```