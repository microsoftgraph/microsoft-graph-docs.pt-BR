---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c64428d45cb7e42b7b3bb67f2168db0ce20ea2d2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116427"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.bookingBusinesses("Contosolunchdelivery@contoso.onmicrosoft.com").services("57da6774-a087-4d69-b0e6-6fb82c339976")
    .buildRequest()
    .delete();

```