---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 00e0de7ffa31f40d4d0aeb924f178c1cdac5591947eb81aaa556abf803dd4ebe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271923"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerRosterMemberCollectionPage members = graphClient.planner().rosters("6519868f-868f-6519-8f86-19658f861965").members()
    .buildRequest()
    .get();

```