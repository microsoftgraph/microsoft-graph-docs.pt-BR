---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d8af89ee6c5af43cc2e273ee4d0bd1e57590dfc3
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48983844"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Boolean securityEnabledOnly = true;

graphClient.servicePrincipals("{id}")
    .getMemberObjects(securityEnabledOnly)
    .buildRequest()
    .post();

```