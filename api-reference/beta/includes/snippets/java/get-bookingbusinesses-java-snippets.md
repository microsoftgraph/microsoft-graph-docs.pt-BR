---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 72142dd1d91c6c594348032f7cdc66840106cedc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969357"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingBusinessCollectionPage bookingBusinesses = graphClient.bookingBusinesses()
    .buildRequest()
    .get();

```