---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 831abb1450b5ff7d4ab341d4244bebb1b237fa4a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959873"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("{id}").calendar().calendarPermissions("{id}")
    .buildRequest()
    .delete();

```