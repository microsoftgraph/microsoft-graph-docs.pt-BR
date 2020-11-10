---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 65c587c80c7587e3a4da8cb0238bfcfbe6aca5d0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979029"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Boolean securityEnabledOnly = true;

graphClient.contacts("{id}")
    .getMemberGroups(securityEnabledOnly)
    .buildRequest()
    .post();

```