---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bd3b17cd8bbf44e5e889ffab6cc8a5b9a4fe41f8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982754"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeViewCollectionPage rows = graphClient.me().drive().root().workbook().worksheets("{id}")
    .range(WorkbookWorksheetRangeParameterSet
        .newBuilder()
        .withAddress("A1:Z10")
        .build())
    .visibleView().rows()
    .buildRequest()
    .get();

```