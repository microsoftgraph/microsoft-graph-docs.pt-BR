---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9a1856c3e75d2e06cc059edcd5e9170fa10f3969
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48958790"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartDataLabels workbookChartDataLabels = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").dataLabels()
    .buildRequest()
    .get();

```