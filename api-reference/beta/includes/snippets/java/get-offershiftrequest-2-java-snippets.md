---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 933853bcce5c8c761de0511b81e80a33688ede1a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946010"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOfferShiftRequestCollectionPage offerShiftRequests = graphClient.teams("{teamId}").schedule().offerShiftRequests()
    .buildRequest()
    .get();

```