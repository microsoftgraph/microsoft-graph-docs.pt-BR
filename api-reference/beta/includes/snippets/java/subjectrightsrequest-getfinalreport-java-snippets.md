---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 718a4d9432be3ae6934f5348e5cedcac926611f4
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60558965"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.privacy().subjectRightsRequests("{subjectRightsRequestId}")
    .getFinalReport()
    .buildRequest()
    .get();

```