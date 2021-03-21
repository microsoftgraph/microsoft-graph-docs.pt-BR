---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 13bde4eceba376edc612d98b9a46c9b9678861d5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983945"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerTaskCollectionPage tasks = graphClient.me().planner().tasks()
    .buildRequest()
    .get();

```