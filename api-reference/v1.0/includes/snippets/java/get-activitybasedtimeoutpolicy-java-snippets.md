---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9c6dbc9fb2d0a67cba9a175e00f38a8c3abc86f2
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806280"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ActivityBasedTimeoutPolicy activityBasedTimeoutPolicy = graphClient.policies().activityBasedTimeoutPolicies("{id}")
    .buildRequest()
    .get();

```