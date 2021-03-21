---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3777076a0302d604635609ffb3efb8c3ca1b224d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971768"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintServiceEndpoint printServiceEndpoint = graphClient.print().services("{printServiceId}").endpoints("{printServiceEndpointId}")
    .buildRequest()
    .get();

```