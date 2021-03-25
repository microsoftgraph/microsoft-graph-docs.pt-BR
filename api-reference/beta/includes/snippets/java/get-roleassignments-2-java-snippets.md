---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3a87368a4b763866e38c5d5bada0dd44f3274544
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210151"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentCollectionPage roleAssignments = graphClient.roleManagement().directory().roleAssignments()
    .buildRequest()
    .get();

```