---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6731447f0f33e553d949833f033f07debf1119be
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095971"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EdiscoveryIndexOperation ediscoveryIndexOperation = graphClient.security().cases().ediscoveryCases("b0073e4e-4184-41c6-9eb7-8c8cc3e2288b").custodians("0053a61a3b6c42738f7606791716a22a").lastIndexOperation()
    .buildRequest()
    .get();

```