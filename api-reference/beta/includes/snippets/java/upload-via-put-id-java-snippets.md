---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c344ceffbf8889c411dcdda035ac2f7c1e1173a3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976628"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

byte[] stream = Base64.getDecoder().decode("The contents of the file goes here.");
    graphClient.me().drive().items("{item-id}")
    .buildRequest()
    .put(stream);

```