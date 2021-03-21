---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c67c884c0f4a64bec2e1ebba4ea9daadf5623bd2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980167"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().root().workbook().worksheets("{id}")
    .range()
    .rowsBelow(WorkbookRangeRowsBelowParameterSet
        .newBuilder()
        .withCount(2)
        .build())
    .buildRequest()
    .get();

```