---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 494e5069def0ffb0e0bbe8905c86bd03347f9553
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959959"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CalendarGroup calendarGroup = graphClient.me().calendarGroups("{id}")
    .buildRequest()
    .get();

```