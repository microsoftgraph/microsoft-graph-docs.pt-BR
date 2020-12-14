---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bae82d2e7337350c4767ede22cf5372bdeb66ca0
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659328"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.compliance().ediscovery().cases("2192ca408ea2410eba3bec8ae873be6b").custodians("45454331323337443946343043464239")
    .activate()
    .buildRequest()
    .post();

```