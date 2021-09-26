---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a766fa0b1b39ee29881c2d2eac318bc99a6a6705023f019f8184727bd0eff955
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272679"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = new Group();
LinkedList<AssignedLabel> assignedLabelsList = new LinkedList<AssignedLabel>();
AssignedLabel assignedLabels = new AssignedLabel();
assignedLabels.labelId = "45cd0c48-c540-4358-ad79-a3658cdc5b88";
assignedLabelsList.add(assignedLabels);
group.assignedLabels = assignedLabelsList;

graphClient.groups("{id}")
    .buildRequest()
    .patch(group);

```