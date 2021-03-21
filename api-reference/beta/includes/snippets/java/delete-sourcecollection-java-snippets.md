---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1628f5ddc59ba7db2262b40f94601763847f0362
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980064"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.compliance().ediscovery().cases("{caseId}").sourceCollections("{sourceCollectionId}")
    .buildRequest()
    .delete();

```