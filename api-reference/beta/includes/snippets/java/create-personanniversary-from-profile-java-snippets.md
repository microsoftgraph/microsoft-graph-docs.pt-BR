---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c321ee9ad9ac38834e4dd38110b5aaaed3a1fa12
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969053"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonAnnualEvent personAnnualEvent = new PersonAnnualEvent();
personAnnualEvent.type = PersonAnnualEventType.BIRTHDAY;
personAnnualEvent.date = new DateOnly(1900,1,1);

graphClient.me().profile().anniversaries()
    .buildRequest()
    .post(personAnnualEvent);

```