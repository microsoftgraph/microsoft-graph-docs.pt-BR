---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bfd0e0ba5600b2bfb863166bd5ba8c25cdcf5b92
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892683"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookTableColumn workbookTableColumn = new WorkbookTableColumn();
workbookTableColumn.id = 99;
workbookTableColumn.name = "name-value";
workbookTableColumn.index = 99;
workbookTableColumn.values = "values-value";

graphClient.me().drive().items("{id}").workbook().tables("{id|name}").columns()
    .buildRequest()
    .post(workbookTableColumn);

```