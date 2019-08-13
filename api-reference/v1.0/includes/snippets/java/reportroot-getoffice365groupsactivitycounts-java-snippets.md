---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 535bfc3d6ea18acb05f087f98d6535dee0c0344a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324699"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOffice365GroupsActivityCounts("D7")
    .buildRequest()
    .get();

```