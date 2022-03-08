---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c2fcec5897dfc743bff57f38f1de37aea54d7e73
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338025"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRbacResourceAction unifiedRbacResourceAction = graphClient.roleManagement().directory().resourceNamespaces("microsoft.directory").resourceActions("microsoft.directory-accessReviews-allProperties-read-get")
    .buildRequest()
    .get();

```