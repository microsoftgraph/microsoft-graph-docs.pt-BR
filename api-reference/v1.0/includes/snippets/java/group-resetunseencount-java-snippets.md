---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d9af667b46037bc313bb7dd74b19000ec574d042
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885358"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{id}")
    .resetUnseenCount()
    .buildRequest()
    .post();

```