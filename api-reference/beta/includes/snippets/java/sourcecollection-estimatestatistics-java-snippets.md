---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 32006a18eec00bc2e6e03ee8b8203acbbaedb7c4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981370"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.compliance().ediscovery().cases("{caseId}").sourceCollections("{sourceCollectionId}")
    .estimateStatistics()
    .buildRequest()
    .post();

```