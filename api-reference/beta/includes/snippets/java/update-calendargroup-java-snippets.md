---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 386de1ff5803a33ef4ead0b5b9345c5a7c737eda8ceefa7a854e9c4cb73a1d6f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214235"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CalendarGroup calendarGroup = new CalendarGroup();
calendarGroup.name = "name-value";

graphClient.me().calendarGroups("{id}")
    .buildRequest()
    .patch(calendarGroup);

```