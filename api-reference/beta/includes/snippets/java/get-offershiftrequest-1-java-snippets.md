---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d74a69651d2f4b1e8253ae33c2b7f5539b8c84af
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210084"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OfferShiftRequest offerShiftRequest = graphClient.teams("{teamId}").schedule().offerShiftRequests("{offerShiftRequestId}")
    .buildRequest()
    .get();

```