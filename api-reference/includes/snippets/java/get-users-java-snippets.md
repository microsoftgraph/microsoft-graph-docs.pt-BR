---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6170c5040dc0c64eb61a57dc16bc4af939b3c716
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35897101"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

User user = graphClient.users("{user-id}")
    .buildRequest()
    .get();

```