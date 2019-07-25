---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 643faa12bdda74e0997cd321c600e094aa2d7a86
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864231"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChart workbookChart = new WorkbookChart();
workbookChart.height = 99;
workbookChart.left = 99;

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}")
    .buildRequest()
    .patch(workbookChart);

```