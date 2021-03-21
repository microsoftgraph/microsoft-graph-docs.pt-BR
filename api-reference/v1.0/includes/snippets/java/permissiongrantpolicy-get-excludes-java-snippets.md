---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: df785dbdec09b30affd3bb671ae4bc0bdce9a84e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976934"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PermissionGrantConditionSetCollectionPage excludes = graphClient.policies().permissionGrantPolicies("microsoft-application-admin").excludes()
    .buildRequest()
    .get();

```