---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7514070d447b49e247cce8f82fee8c47182f8536
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49944921"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPlannerBucketCollectionPage buckets = graphClient.planner().buckets()
    .buildRequest()
    .get();

```