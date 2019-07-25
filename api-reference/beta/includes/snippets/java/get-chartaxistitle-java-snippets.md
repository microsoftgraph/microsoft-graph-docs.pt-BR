---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 170465948d640dc5879c553d751c0319f1651923
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864181"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartAxisTitle workbookChartAxisTitle = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").axes().valueAxis().title()
    .buildRequest()
    .get();

```