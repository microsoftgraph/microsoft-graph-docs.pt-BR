---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1dcc6bb41d299a38296cef32c3549a6f2e5f910e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62109677"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingCustomQuestion bookingCustomQuestion = graphClient.bookingBusinesses("Contosolunchdelivery@contoso.onmicrosoft.com").customQuestions("3bc6fde0-4ad3-445d-ab17-0fc15dba0774")
    .buildRequest()
    .get();

```