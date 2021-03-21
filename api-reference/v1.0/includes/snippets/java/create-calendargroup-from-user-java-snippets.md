---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4cf848147c11ee2c5bd60b68966604fd4a4bb299
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970669"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CalendarGroup calendarGroup = new CalendarGroup();
calendarGroup.name = "name-value";
calendarGroup.classId = UUID.fromString("classId-value");
calendarGroup.changeKey = "changeKey-value";

graphClient.me().calendarGroups()
    .buildRequest()
    .post(calendarGroup);

```