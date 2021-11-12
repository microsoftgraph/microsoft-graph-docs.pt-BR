---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 206e42dd2d7735156b001a1332bb11f010a98d6d14f766815eeca697266bd90b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101442"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeView workbookRangeView = graphClient.drive().root().workbook().worksheets("{id}")
    .range(WorkbookWorksheetRangeParameterSet
        .newBuilder()
        .withAddress("A1:Z10")
        .build())
    .visibleView()
    .buildRequest()
    .get();

```