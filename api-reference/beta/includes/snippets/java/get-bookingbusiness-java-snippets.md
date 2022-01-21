---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4230bb1718d898f77c45be681060fac0b6ba858e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116497"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingBusiness bookingBusiness = graphClient.bookingBusinesses("Fabrikam@contoso.onmicrosoft.com")
    .buildRequest()
    .get();

```