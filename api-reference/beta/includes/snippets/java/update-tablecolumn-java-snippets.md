---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f1947e83629e7acb5ec1a8bcdfd3939dade09899
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35868605"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookTableColumn workbookTableColumn = new WorkbookTableColumn();
workbookTableColumn.name = "name-value";
workbookTableColumn.index = 99;
workbookTableColumn.values = "values-value";

graphClient.me().drive().items("{id}").workbook().tables("{id|name}").columns("{id|name}")
    .buildRequest()
    .patch(workbookTableColumn);

```