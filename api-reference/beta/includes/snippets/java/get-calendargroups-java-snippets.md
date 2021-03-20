---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3df7d99f1457796d7f4154c0f21101efa2b34b83
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974931"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CalendarGroupCollectionPage calendarGroups = graphClient.me().calendarGroups()
    .buildRequest()
    .get();

```