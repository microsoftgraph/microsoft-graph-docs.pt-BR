---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 20af2ec48f631d3364794e489df51971c874321e0e30ee08f82d5fe5f4e448d2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273257"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "return=representation"));

SchedulingGroup schedulingGroup = new SchedulingGroup();
schedulingGroup.displayName = "Cashiers";
schedulingGroup.isActive = true;
LinkedList<String> userIdsList = new LinkedList<String>();
userIdsList.add("c5d0c76b-80c4-481c-be50-923cd8d680a1");
userIdsList.add("2a4296b3-a28a-44ba-bc66-0274b9b95851");
schedulingGroup.userIds = userIdsList;

graphClient.teams("{teamId}").schedule().schedulingGroups("{schedulingGroupId}")
    .buildRequest( requestOptions )
    .put(schedulingGroup);

```