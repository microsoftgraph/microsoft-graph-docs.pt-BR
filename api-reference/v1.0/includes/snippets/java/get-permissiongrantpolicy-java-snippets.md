---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 716a0c4b8c7c2e31111ed97f73da2d3f1799d45e
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524470"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PermissionGrantPolicy permissionGrantPolicy = graphClient.policies().permissionGrantPolicies("microsoft-user-default-low")
    .buildRequest()
    .get();

```