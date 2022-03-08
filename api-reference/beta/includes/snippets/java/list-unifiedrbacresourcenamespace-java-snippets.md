---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9149802f212e0cf898e02889e2fa7e22d0014d1e
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338124"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRbacResourceNamespaceCollectionPage resourceNamespaces = graphClient.roleManagement().directory().resourceNamespaces()
    .buildRequest()
    .get();

```