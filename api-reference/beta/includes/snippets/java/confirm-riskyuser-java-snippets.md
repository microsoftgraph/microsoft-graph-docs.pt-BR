---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7773bbb4fc85d8e9638d610bb0022e55ff16b0bd
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871035"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> userIdsList = new LinkedList<String>();
userIdsList.add("29f270bb-4d23-4f68-8a57-dc73dc0d4caf");
userIdsList.add("20f91ec9-d140-4d90-9cd9-f618587a1471");

graphClient.riskyUsers()
    .confirmCompromised(userIdsList)
    .buildRequest()
    .post();

```