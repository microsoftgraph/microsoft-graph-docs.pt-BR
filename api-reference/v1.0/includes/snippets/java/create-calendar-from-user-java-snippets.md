---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 09b3771037fb7520c7d5c2eaa8e5f43e2a287a19
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882753"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Calendar calendar = new Calendar();
calendar.name = "Volunteer";

graphClient.me().calendars()
    .buildRequest()
    .post(calendar);

```