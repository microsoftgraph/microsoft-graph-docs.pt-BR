---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 867e064171878a2d487b41e743dbca169822abcd
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321831"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSharePointActivityUserCounts("D7")
    .buildRequest()
    .get();

```