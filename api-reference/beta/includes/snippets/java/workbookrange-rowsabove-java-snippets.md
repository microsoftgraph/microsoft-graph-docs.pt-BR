---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 274a0fa22502b62ce0991e25010fd9aa498d3d6442ce401c6d271b960ca545a2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157350"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.drive().root().workbook().worksheets("{id}")
    .range()
    .rowsAbove(WorkbookRangeRowsAboveParameterSet
        .newBuilder()
        .withCount(2)
        .build())
    .buildRequest()
    .get();

```