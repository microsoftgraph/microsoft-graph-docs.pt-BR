---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5575a3377f71dd49735923e512df74f75fab0342
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980304"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LegalHoldCollectionPage legalHolds = graphClient.compliance().ediscovery().cases("{caseId}").legalHolds()
    .buildRequest()
    .get();

```