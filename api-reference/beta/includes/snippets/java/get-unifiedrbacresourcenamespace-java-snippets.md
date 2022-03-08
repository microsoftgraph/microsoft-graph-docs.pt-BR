---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8d85c1930a2a586fe614d257a74a0e4341b1130c
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338413"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRbacResourceNamespace unifiedRbacResourceNamespace = graphClient.roleManagement().directory().resourceNamespaces("microsoft.aad.b2c")
    .buildRequest()
    .get();

```