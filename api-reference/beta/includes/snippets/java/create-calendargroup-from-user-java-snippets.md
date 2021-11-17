---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c28e6649b50cab90cafe962c2c221f2476fec19ec43d345f9e5d621823d8f867
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329544"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CalendarGroup calendarGroup = new CalendarGroup();
calendarGroup.name = "Personal events";

graphClient.me().calendarGroups()
    .buildRequest()
    .post(calendarGroup);

```