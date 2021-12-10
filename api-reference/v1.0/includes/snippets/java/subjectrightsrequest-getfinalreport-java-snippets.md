---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 718a4d9432be3ae6934f5348e5cedcac926611f4
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687568"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.privacy().subjectRightsRequests("{subjectRightsRequestId}")
    .getFinalReport()
    .buildRequest()
    .get();

```