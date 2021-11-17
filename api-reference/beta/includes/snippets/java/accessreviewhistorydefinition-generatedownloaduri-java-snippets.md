---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 010e7a9eddedd4fedcbca62db4591040dc40f06d259e0d985cb54790af075c7f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898221"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().accessReviews().historyDefinitions("b2cb022f-b7e1-40f3-9854-c65a40861c38")
    .generateDownloadUri()
    .buildRequest()
    .post();

```