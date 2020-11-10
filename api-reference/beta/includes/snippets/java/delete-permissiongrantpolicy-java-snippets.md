---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 44bc3352dc2bd10656a00b805d22a9a1ac602f4e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977942"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().permissionGrantPolicies("my-custom-consent-policy")
    .buildRequest()
    .delete();

```