---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6abf3ce3a5e64c056a66ce1e849f7dba53632bf34ca77740289decfd439209d1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273361"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.compliance().ediscovery().cases("{caseId}").legalHolds("{legalholdId}")
    .buildRequest()
    .delete();

```