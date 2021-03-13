---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cc0e5388985ea8dd5b9724c31725a192f50f1bb3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774009"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().termsOfUse().agreements("{id}")
    .buildRequest()
    .delete();

```