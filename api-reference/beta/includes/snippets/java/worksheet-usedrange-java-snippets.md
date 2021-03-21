---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7adf2a2fc2ee10c7d8a1cb02c43642c250b4a14c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979091"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}")
    .usedRange(WorkbookWorksheetUsedRangeParameterSet
        .newBuilder()
        .withValuesOnly(true)
        .build())
    .buildRequest()
    .get();

```