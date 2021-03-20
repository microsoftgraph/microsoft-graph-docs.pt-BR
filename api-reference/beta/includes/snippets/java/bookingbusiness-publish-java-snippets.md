---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 63c04e0bcbaee6cbd9c346798e9bcff0d72fd042
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977186"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com")
    .publish()
    .buildRequest()
    .post();

```