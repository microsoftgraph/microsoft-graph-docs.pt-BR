---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dbb972a2321d1fbf34630016405283db604b9fb5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970521"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartFont workbookChartFont = new WorkbookChartFont();
workbookChartFont.bold = true;
workbookChartFont.color = "color-value";
workbookChartFont.italic = true;
workbookChartFont.name = "name-value";
workbookChartFont.size = 99d;
workbookChartFont.underline = "underline-value";

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").axes().valueAxis().format().font()
    .buildRequest()
    .patch(workbookChartFont);

```