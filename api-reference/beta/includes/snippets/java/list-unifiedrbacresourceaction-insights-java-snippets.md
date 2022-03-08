---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 21f1359ea773bddaca2fc19628c4f91e1d7e93e5
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337975"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRbacResourceActionCollectionPage resourceActions = graphClient.roleManagement().directory().resourceNamespaces("microsoft.insights").resourceActions()
    .buildRequest()
    .get();

```