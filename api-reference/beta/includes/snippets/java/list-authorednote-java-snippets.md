---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fb0d5a50a595ff50f695fc2e83b1d7fa384cfd6f
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60558590"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthoredNoteCollectionPage notes = graphClient.privacy().subjectRightsRequests("{subjectRightsRequestId}").notes()
    .buildRequest()
    .get();

```