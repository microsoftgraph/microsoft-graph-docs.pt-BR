---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a57821372def151be38bcb3edc2066b0790277f7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969708"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().connectors("{printConnectorId}")
    .buildRequest()
    .delete();

```