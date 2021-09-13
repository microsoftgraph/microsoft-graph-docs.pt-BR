---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b52fe8a375951146add1b8f42aa217e7e7e97a809bf5a74990d51efee57ca2b1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273590"
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