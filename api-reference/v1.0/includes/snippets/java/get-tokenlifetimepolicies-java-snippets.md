---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: beb4b22d92af23999c8d21789693f00925482956
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43718542"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITokenLifetimePolicyCollectionPage tokenLifetimePolicies = graphClient.policies().tokenLifetimePolicies()
    .buildRequest()
    .get();

```