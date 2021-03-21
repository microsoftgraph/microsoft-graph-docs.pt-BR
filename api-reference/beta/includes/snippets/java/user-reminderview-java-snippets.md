---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 925c5ed6aa35d89211a033bcf65a7fc748fb99b2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983016"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserReminderViewCollectionPage reminderView = graphClient.me()
    .reminderView(UserReminderViewParameterSet
        .newBuilder()
        .withStartDateTime("2017-06-05T10:00:00.0000000")
        .withEndDateTime("2017-06-11T11:00:00.0000000")
        .build())
    .buildRequest()
    .get();

```