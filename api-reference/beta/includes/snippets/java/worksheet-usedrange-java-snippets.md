---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 56c2a0ec6e6a09344e3d5a9ba600275eb3fb20a08af54d313b916e518b8c8715
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215034"
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