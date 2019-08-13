---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a7761d3e944b3a67b6b7aa045d0bf5376b1a8056
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320622"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSkypeForBusinessPeerToPeerActivityCounts("D7")
    .buildRequest()
    .get();

```