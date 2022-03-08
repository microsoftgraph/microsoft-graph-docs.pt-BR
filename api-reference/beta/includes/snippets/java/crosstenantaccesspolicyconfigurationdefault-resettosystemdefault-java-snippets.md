---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 21cae7adcf12214c505edfa8adc08c07dc4efe95
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336435"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().crossTenantAccessPolicy().default()
    .resetToSystemDefault()
    .buildRequest()
    .post();

```