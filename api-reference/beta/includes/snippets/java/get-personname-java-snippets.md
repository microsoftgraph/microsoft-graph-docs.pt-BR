---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d6a1c97813a61080aab6bc0d8a46016b09b7af6f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967710"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonName personName = graphClient.me().profile().names("{id}")
    .buildRequest()
    .get();

```