---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3f7c5c3c66cd820043abc2a798a77a025c1c8235
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947024"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String contentType = "https://graph.microsoft.com/beta/sites/id/contentTypes/0x0101";

graphClient.sites("id").lists("{list-id}").contentTypes()
    .addCopy(ContentTypeAddCopyParameterSet
        .newBuilder()
        .withContentType(contentType)
        .build())
    .buildRequest()
    .post();

```