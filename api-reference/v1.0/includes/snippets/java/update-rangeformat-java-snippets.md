---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5678ddb2cd6ef45f7152cc2c0c54077fd744005d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324733"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFormat workbookRangeFormat = new WorkbookRangeFormat();
workbookRangeFormat.columnWidth = 135;
workbookRangeFormat.verticalAlignment = "Top";
workbookRangeFormat.rowHeight = 49;
workbookRangeFormat.wrapText = false;

graphClient.me().drive().items("{id}").workbook().worksheets("{sheet-id}")
    .range("$A$1").format()
    .buildRequest()
    .patch(workbookRangeFormat);

```