---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 184775936bf65094c8f0f9d51b7a5d31ad560a95
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524303"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPermissionGrantConditionSetCollectionPage includes = graphClient.policies().permissionGrantPolicies("microsoft-application-admin").includes()
    .buildRequest()
    .get();

```