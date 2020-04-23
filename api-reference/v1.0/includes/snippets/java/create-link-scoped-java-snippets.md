---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 40526a28a9c573fd5e7bf26389d182490f3bc024
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43771034"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String type = "edit";

String scope = "organization";

graphClient.me().drive().items("{item-id}")
    .createLink(type,scope,null,null,null)
    .buildRequest()
    .post();

```