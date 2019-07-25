---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 91b9c95fafaa898fd5286bee6803a1d4a142f748
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864294"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartSeries workbookChartSeries = new WorkbookChartSeries();
workbookChartSeries.name = "name-value";

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").series()
    .buildRequest()
    .post(workbookChartSeries);

```