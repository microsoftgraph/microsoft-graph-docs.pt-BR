---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ff9d1688f5fab4630221eee2820c8f3857d0c60d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975239"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CalendarCollectionPage calendars = graphClient.me().calendars()
    .buildRequest()
    .get();

```