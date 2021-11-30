---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ff95b4ef8f05aa3fed40df866ed59c3782f31761
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61224994"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> groupIdsList = new LinkedList<String>();
groupIdsList.add("fee2c45b-915a-4a64-b130-f4eb9e75525e");
groupIdsList.add("4fe90ae7-065a-478b-9400-e0a0e1cbd540");

graphClient.me()
    .checkMemberGroups(DirectoryObjectCheckMemberGroupsParameterSet
        .newBuilder()
        .withGroupIds(groupIdsList)
        .build())
    .buildRequest()
    .post();

```