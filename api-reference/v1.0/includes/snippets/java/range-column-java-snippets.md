---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b4ee5137b2ec0cc82dc6b0e2fd447613ec8be3cd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968491"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .column(WorkbookRangeColumnParameterSet
        .newBuilder()
        .withColumn(5)
        .build())
    .buildRequest()
    .get();

```