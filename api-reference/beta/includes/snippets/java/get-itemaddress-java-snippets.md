---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bff1fba0fddc8ea275afa2922b48a03a52d0883d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969448"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemAddress itemAddress = graphClient.me().profile().addresses("{id}")
    .buildRequest()
    .get();

```