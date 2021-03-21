---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 69b7514a04e0aeb9b22259b2833b8d2c912aa6d5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975388"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.customRequest("/me/onenote/resources/{id}/content", InputStream.class)
    .buildRequest()
    .get();

```