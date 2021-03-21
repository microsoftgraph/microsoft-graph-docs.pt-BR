---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6cdb7317708ce725736a1d7014a19145ca631d3e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980979"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingBusiness bookingBusiness = graphClient.bookingBusinesses("Fabrikam@M365B489948.onmicrosoft.com")
    .buildRequest()
    .get();

```