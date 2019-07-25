---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3740862f18dd5e39850a3077ad12dac1ca9439d2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860209"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("11021").assignments("19002").submissions("850f51b7")
    .submit()
    .buildRequest()
    .post();

```