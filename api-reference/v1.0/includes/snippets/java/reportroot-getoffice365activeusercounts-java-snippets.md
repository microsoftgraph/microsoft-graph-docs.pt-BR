---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d42b99f54b62273b767c71240a82e72fb884bb57
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327113"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOffice365ActiveUserCounts("D7")
    .buildRequest()
    .get();

```