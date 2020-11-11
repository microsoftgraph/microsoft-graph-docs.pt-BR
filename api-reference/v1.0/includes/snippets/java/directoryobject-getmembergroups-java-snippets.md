---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5734f6d5c446ded717a8595c70699bda12f1849f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48982944"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Boolean securityEnabledOnly = true;

graphClient.directoryObjects("{object-id}")
    .getMemberGroups(securityEnabledOnly)
    .buildRequest()
    .post();

```