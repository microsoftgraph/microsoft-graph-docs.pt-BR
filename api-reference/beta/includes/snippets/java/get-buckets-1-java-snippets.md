---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b67ff3d1827fd09ccceee48e9631e4932458fbe4634aca9889860a0f5caec345
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217388"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerBucketCollectionPage buckets = graphClient.planner().buckets()
    .buildRequest()
    .get();

```