---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d1f62b87b854bb3a434f32645f06eb2e416d3d94
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092338"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.security().cases().ediscoveryCases("b0073e4e-4184-41c6-9eb7-8c8cc3e2288b").custodians("c25c3914f9f743ee9cbaa25377e0cec6")
    .release()
    .buildRequest()
    .post();

```