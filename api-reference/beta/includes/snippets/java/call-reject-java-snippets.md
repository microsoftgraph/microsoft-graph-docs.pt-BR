---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4c9fb4e28ef1c9aea008c7a054f90d34ea7152c0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864597"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RejectReason reason = RejectReason.NONE;

graphClient.app().calls("{id}")
    .reject(reason)
    .buildRequest()
    .post();

```