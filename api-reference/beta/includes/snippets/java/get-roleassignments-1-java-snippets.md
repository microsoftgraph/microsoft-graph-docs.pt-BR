---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 847554b2e3198c5e740b4594c8e87fe0b09d3edf
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210888"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentCollectionPage roleAssignments = graphClient.roleManagement().directory().roleAssignments()
    .buildRequest()
    .filter("roleDefinitionId eq '62e90394-69f5-4237-9190-012177145e10'")
    .expand("principal")
    .get();

```