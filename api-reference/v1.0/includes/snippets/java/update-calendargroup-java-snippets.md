---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b98e0b3a630847ed527d836301820762a9e83cf9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882326"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CalendarGroup calendarGroup = new CalendarGroup();
calendarGroup.name = "name-value";

graphClient.me().calendarGroups("{id}")
    .buildRequest()
    .patch(calendarGroup);

```