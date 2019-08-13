---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a5d9f5a6e4da04a7de2e7421121e40ca719c0f0b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36362447"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEmailAddressCollectionPage findRooms = graphClient.me()
    .findRooms("Building2Rooms@contoso.onmicrosoft.com")
    .buildRequest()
    .get();

```