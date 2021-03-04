---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7b8ffdf60bea066e9236886b313ad77064999e34
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447857"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String message = "message-value";

graphClient.teams("{id}").schedule().openShiftChangeRequests("{openShiftChangeRequestId}")
    .decline(message)
    .buildRequest()
    .post();

```