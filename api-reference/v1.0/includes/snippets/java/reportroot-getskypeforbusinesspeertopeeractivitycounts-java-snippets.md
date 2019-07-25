---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e2850a31da44764765aa5d7f79ac1892e27bac9b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892227"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSkypeForBusinessPeerToPeerActivityCounts('D7')
    .buildRequest()
    .get();

```