---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 86f3ba2a3a13c6a4152b5f8ad7c575a3110fe00f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867702"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEmailAddressCollectionPage findRooms = graphClient.me()
    .findRooms('Building2Rooms@contoso.onmicrosoft.com')
    .buildRequest()
    .get();

```