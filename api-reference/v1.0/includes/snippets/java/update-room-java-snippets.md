---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6a9756bd048035d2dfd513825e49e8b281be6300
ms.sourcegitcommit: 1138d6e84f64f3727e180da10f89b89021855c3e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2021
ms.locfileid: "50059614"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Room place = new Room();
place.nickname = "Conf Room";
place.building = "1";
place.label = "100";
place.capacity = 50;
place.isWheelChairAccessible = false;

graphClient.places("cf100@contoso.com")
    .buildRequest()
    .patch(place);

```