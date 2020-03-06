---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6646acae95813b554cf68a717a24854fb31ec1a9
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638379"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> groupIdsList = new LinkedList<String>();
groupIdsList.add("groupId-value1");
groupIdsList.add("groupId-value2");

graphClient.contacts("{id}")
    .checkMemberGroups(groupIdsList)
    .buildRequest()
    .post();

```