---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e21e7bbc834c4d4e8b66c7e332ad3d3104a631b3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865386"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com").customers("80b5ddda-1e3b-4c9d-abe2-d606cc075e2e")
    .buildRequest()
    .delete();

```