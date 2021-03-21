---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b2e5ec80be3c8458b2355badb2c76d4afd0dfd8e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982309"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AlertCollectionPage alerts = graphClient.security().alerts()
    .buildRequest()
    .get();

```