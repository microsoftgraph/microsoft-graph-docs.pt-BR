---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f1781cbbf7cb20f8b4a820e251391ff051b1d351
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327309"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getEmailAppUsageUserDetail("D7")
    .buildRequest()
    .get();

```