---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d4922da4bbfbafc86b1f3d773a68a28a7f6aa487
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239151"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DeploymentCollectionPage deployments = graphClient.admin().windows().updates().deployments()
    .buildRequest()
    .get();

```