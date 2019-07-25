---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5dec5f121476bd5247f85d7dc35484a062d5dbad
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893309"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> groupIdsList = new LinkedList<String>();
groupIdsList.add("fee2c45b-915a-4a64b130f4eb9e75525e");
groupIdsList.add("4fe90ae065a-478b9400e0a0e1cbd540");

graphClient.directoryObjects("{id}")
    .checkMemberGroups(groupIdsList)
    .buildRequest()
    .post();

```