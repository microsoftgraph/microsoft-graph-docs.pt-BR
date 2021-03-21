---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7514070d447b49e247cce8f82fee8c47182f8536
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962887"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPlannerBucketCollectionPage buckets = graphClient.planner().buckets()
    .buildRequest()
    .get();

```