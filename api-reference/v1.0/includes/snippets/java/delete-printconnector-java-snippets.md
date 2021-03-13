---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5823323e88f212c5b66a5551f331c757b230c0ba
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772146"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().connectors("{printConnectorId}")
    .buildRequest()
    .delete();

```