---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d8ed77d4f439f213d6b5befd3258d7c2ac3c47a3
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337560"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().accessReviews().historyDefinitions("b2cb022f-b7e1-40f3-9854-c65a40861c38").instances("b2cb022f-b7e1-40f3-9854-c65a40861c38")
    .generateDownloadUri()
    .buildRequest()
    .post();

```