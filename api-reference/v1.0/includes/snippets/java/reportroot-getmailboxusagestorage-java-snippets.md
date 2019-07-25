---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f61ec6e567773977e018585af2f46c5a25adc0d2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888502"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getMailboxUsageStorage('D7')
    .buildRequest()
    .get();

```