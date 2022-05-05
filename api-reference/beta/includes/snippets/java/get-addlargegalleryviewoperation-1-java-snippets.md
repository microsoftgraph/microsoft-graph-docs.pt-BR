---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1807bbdfa870077f6a45b0447c7db308e3eecc07
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204156"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CommsOperation commsOperation = graphClient.communications().calls("57dab8b1-894c-409a-b240-bd8beae78896").operations("e33176d4-836a-4fd7-b95a-d11bda52811d")
    .buildRequest()
    .get();

```