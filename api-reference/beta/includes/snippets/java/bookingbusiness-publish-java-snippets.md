---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 18a1d02c276a0826ea9617f988de362326abaefe
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137580"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.bookingBusinesses("Contosolunchdelivery@contoso.onmicrosoft.com")
    .publish()
    .buildRequest()
    .post();

```