---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b4ff8a60adc05d4cb4dd604a1e9f90c83c8fac0c
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508901"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().featureRolloutPolicies("df85e4d9-e8c4-4033-a41c-73419a95c29c")
    .buildRequest()
    .delete();

```