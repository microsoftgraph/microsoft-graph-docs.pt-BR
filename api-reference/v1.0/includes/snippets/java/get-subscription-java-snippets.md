---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 85a6f640368cf0c89ba258eed3ef3d01480a5674
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982593"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Subscription subscription = graphClient.subscriptions("{id}")
    .buildRequest()
    .get();

```