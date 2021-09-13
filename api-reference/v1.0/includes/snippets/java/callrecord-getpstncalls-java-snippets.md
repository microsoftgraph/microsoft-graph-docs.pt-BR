---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 006e91f121540123c573c1dbe521add459a7fac9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59056849"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CallRecord callRecord = graphClient.communications().callRecords("getPstnCalls(fromDateTime=2019-11-01,toDateTime=2019-12-01)")
    .buildRequest()
    .get();

```