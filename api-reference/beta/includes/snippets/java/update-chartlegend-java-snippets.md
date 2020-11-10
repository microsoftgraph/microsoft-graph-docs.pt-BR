---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 59a0854de6d37549305ac979e56818fac81b30d6
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48958609"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartLegend workbookChartLegend = new WorkbookChartLegend();
workbookChartLegend.visible = true;
workbookChartLegend.position = "position-value";
workbookChartLegend.overlay = true;

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").legend()
    .buildRequest()
    .patch(workbookChartLegend);

```