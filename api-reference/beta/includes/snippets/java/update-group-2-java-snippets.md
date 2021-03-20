---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4b02226da869280f3069f847788c4c39211f0a87
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944217"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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