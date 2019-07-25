---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9a845bf2801927fa439721eaa3e14cdb3d9215ba
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867891"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> groupIdsList = new LinkedList<String>();
groupIdsList.add("groupIds-value");

graphClient.me()
    .checkMemberGroups(groupIdsList)
    .buildRequest()
    .post();

```