---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7dceba47b2cd26fbf469bc8c754075e26a77ef07
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35868830"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().tables("{id|name}")
    .range()
    .buildRequest()
    .post();

```