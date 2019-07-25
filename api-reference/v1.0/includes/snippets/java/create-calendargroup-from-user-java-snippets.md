---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9df55d7923c30756cff84c389018c126f909b4cb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882782"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CalendarGroup calendarGroup = new CalendarGroup();
calendarGroup.name = "name-value";
calendarGroup.classId = "classId-value";
calendarGroup.changeKey = "changeKey-value";

graphClient.me().calendarGroups()
    .buildRequest()
    .post(calendarGroup);

```