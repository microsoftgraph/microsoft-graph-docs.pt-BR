---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9613511054ed8bee111795fadcfbbce27e533709
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969294"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerTask plannerTask = graphClient.planner().tasks("{task-id}")
    .buildRequest()
    .get();

```