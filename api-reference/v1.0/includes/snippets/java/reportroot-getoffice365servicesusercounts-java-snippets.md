---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d4d54cae9fa3bb88838f4037a114ea08e5b6239a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374369"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOffice365ServicesUserCounts("D7")
    .buildRequest()
    .get();

```