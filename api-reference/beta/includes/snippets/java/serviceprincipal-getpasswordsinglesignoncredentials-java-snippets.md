---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4bd8651e3a7b260db727b6f04c309d804782f271
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980639"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String id = "5793aa3b-cca9-4794-679a240f8b58";

graphClient.servicePrincipals("{id}")
    .getPasswordSingleSignOnCredentials(id)
    .buildRequest()
    .post();

```