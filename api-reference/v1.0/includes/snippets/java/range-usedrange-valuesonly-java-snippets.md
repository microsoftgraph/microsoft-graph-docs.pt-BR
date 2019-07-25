---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 12d1376bb44db1ac1fe3850cae16c22abc408948
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888579"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .usedRange(true)
    .buildRequest()
    .get();

```