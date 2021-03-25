---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 952ac513ef82c75aadf84d10f9482fdde7ef2d6b
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210712"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentMultipleCollectionPage roleAssignments = graphClient.roleManagement().deviceManagement().roleAssignments()
    .buildRequest()
    .get();

```