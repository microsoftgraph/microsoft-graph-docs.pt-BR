---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 01c3a5689e91bdf64934fd6f3a5b03a98cdf65da
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959847"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CalendarPermission calendarPermission = graphClient.users("{id}").calendar().calendarPermissions("{id}")
    .buildRequest()
    .get();

```