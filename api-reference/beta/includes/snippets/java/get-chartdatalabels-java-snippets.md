---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9a1856c3e75d2e06cc059edcd5e9170fa10f3969
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864104"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartDataLabels workbookChartDataLabels = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").dataLabels()
    .buildRequest()
    .get();

```