---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0590d5d6626b85aeb8a06336f91192dc77431d84
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974035"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingCurrencyCollectionPage bookingCurrencies = graphClient.bookingCurrencies()
    .buildRequest()
    .get();

```