---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 552904a533e590df1326eeaefe89185583030626
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209247"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SwapShiftsChangeRequest swapShiftsChangeRequest = graphClient.teams("{teamId}").schedule().swapShiftsChangeRequests("{swapShiftsChangeRequestId}")
    .buildRequest()
    .get();

```