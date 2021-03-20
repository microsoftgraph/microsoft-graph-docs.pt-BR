---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 442798dcebf4a3c70a471269cb1ac006ff3b0393
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945900"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPlannerBucketCollectionPage buckets = graphClient.planner().plans("2txjA-BMZEq-bKi6Wfj5aGQAB1OJ").buckets()
    .buildRequest()
    .get();

```