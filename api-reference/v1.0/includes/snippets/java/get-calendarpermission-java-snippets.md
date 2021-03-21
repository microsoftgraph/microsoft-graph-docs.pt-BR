---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a8d0374f6ea9eb7aa8be342e057c61c42956c71e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982222"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CalendarPermission calendarPermission = graphClient.users("{id}").calendar().calendarPermissions("{id}")
    .buildRequest()
    .get();

```