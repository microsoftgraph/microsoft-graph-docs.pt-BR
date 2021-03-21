---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f9ed6e3610d981d2f260f285415b238a02ae20cd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971785"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String webUrl = "webUrl value";

graphClient.me().onenote().notebooks()
    .getNotebookFromWebUrl(NotebookGetNotebookFromWebUrlParameterSet
        .newBuilder()
        .withWebUrl(webUrl)
        .build())
    .buildRequest()
    .post();

```