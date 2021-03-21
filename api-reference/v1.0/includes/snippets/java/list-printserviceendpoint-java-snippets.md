---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4d5776696944eea0475319830aa76cb5ff3a7f6d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983115"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintServiceEndpointCollectionPage endpoints = graphClient.print().services("{printServiceId}").endpoints()
    .buildRequest()
    .get();

```