---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 46b8cce8c5838fcbc191b50cd5be5a747136a092
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44215791"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITimeOffRequestCollectionPage timeOffRequests = graphClient.teams("{teamId}").schedule().timeOffRequests()
    .buildRequest()
    .get();

```