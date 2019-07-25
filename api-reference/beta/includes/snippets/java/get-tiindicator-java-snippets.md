---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e8f2556bbe5f7af94fb15495ab7abdea1cb87b64
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35868213"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TiIndicator tiIndicator = graphClient.security().tiIndicators("{id}")
    .buildRequest()
    .get();

```