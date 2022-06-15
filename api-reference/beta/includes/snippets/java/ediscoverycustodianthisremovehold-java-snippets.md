---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bec03cd2ed62e7d8c5e8e65c9e9f8723cdcc34ed
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093750"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.security().cases().ediscoveryCases("b0073e4e-4184-41c6-9eb7-8c8cc3e2288b").custodians("c25c3914f9f743ee9cbaa25377e0cec6")
    .removeHold()
    .buildRequest()
    .post();

```