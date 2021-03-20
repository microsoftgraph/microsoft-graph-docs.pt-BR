---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f018ab24369730948c940362b8167aec09be9876
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978226"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerTaskCollectionPage tasks = graphClient.planner().buckets("gcrYAaAkgU2EQUvpkNNXLGQAGTtu").tasks()
    .buildRequest()
    .get();

```