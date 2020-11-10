---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4231696afa691226ff1690948be0bb39c98b5b87
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973086"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookWorksheetProtectionOptions options = new WorkbookWorksheetProtectionOptions();
options.allowFormatCells = true;
options.allowFormatColumns = true;
options.allowFormatRows = true;
options.allowInsertColumns = true;
options.allowInsertRows = true;
options.allowInsertHyperlinks = true;
options.allowDeleteColumns = true;
options.allowDeleteRows = true;
options.allowSort = true;
options.allowAutoFilter = true;
options.allowPivotTables = true;

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").protection()
    .protect(options)
    .buildRequest()
    .post();

```