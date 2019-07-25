---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6e3e0d014d338a0ab58f8cad8721a085b1277ae9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888473"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groupLifecyclePolicies("{id}")
    .buildRequest()
    .delete();

```