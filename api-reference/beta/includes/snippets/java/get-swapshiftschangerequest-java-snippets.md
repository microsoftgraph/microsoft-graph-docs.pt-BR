---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fa020232bafc4ce4471d5ccdef4df5bd4cffbc6f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971931"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISwapShiftsChangeRequestCollectionPage swapShiftsChangeRequests = graphClient.teams("{teamId}").schedule().swapShiftsChangeRequests()
    .buildRequest()
    .get();

```