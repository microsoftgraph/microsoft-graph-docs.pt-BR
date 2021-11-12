---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a0e796b5649ef1aa8559fd0c8476c9098df6767cd4d45adb5c749f91ccb24b77
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159813"
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