---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fc9112c25c3bce9e4cd4f58929dfa0d50924c839
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977394"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.print().printers("{printerId}").jobs("{printJobId}").documents("{printDocumentId}").content()
    .buildRequest()
    .get();

```