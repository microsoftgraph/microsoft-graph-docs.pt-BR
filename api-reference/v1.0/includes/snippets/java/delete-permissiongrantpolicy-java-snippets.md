---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 44bc3352dc2bd10656a00b805d22a9a1ac602f4e
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524331"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().permissionGrantPolicies("my-custom-consent-policy")
    .buildRequest()
    .delete();

```