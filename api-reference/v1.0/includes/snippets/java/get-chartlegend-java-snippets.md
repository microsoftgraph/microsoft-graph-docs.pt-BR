---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ed604542baad909cd11971f0cfd1e9fe2963426e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881928"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartLegend workbookChartLegend = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").legend()
    .buildRequest()
    .get();

```