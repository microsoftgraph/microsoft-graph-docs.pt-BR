---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a04ebcf90c7180cbc8068ceaea954497057a3233
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954316"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{id}").appRoleAssignments("{id}")
    .buildRequest()
    .delete();

```