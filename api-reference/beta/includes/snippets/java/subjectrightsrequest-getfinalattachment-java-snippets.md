---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9cfb1f66e5a1bacaed6ee56506f17c5b9dd896e5
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60559636"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.privacy().subjectRightsRequests("{subjectRightsRequestId}")
    .getFinalAttachment()
    .buildRequest()
    .get();

```