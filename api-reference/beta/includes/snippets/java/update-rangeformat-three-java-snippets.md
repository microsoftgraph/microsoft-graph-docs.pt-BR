---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b9c464c6edc4239da649ed9eac9a47787f4e582869783399bd56ab7cbca06fe3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102256"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFormat workbookRangeFormat = new WorkbookRangeFormat();
workbookRangeFormat.columnWidth = 135d;
workbookRangeFormat.horizontalAlignment = "Right";
workbookRangeFormat.verticalAlignment = "Top";
workbookRangeFormat.rowHeight = 49d;
workbookRangeFormat.wrapText = false;

graphClient.me().drive().items("{id}").workbook().worksheets("Sheet1")
    .range(WorkbookWorksheetRangeParameterSet
        .newBuilder()
        .withAddress("$C$1")
        .build()).format()
    .buildRequest()
    .patch(workbookRangeFormat);

```