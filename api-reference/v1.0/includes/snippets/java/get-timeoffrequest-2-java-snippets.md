---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 46b8cce8c5838fcbc191b50cd5be5a747136a092
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963540"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITimeOffRequestCollectionPage timeOffRequests = graphClient.teams("{teamId}").schedule().timeOffRequests()
    .buildRequest()
    .get();

```