---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 37ef6a83b3c5785571a16fd873edc332671d7f79
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979645"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = new Group();
group.description = "Self help community for library";
group.displayName = "Library Assist";
LinkedList<String> groupTypesList = new LinkedList<String>();
groupTypesList.add("Unified");
group.groupTypes = groupTypesList;
group.mailEnabled = true;
group.mailNickname = "library";
group.securityEnabled = false;

graphClient.groups()
    .buildRequest()
    .post(group);

```