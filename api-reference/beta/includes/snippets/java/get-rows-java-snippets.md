---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 11f91912cdafec4d9bc627bbcc69662acb4c38406451a7e6762608e00fe737ea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217365"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeViewCollectionPage rows = graphClient.drive().root().workbook().worksheets("{id}")
    .range(WorkbookWorksheetRangeParameterSet
        .newBuilder()
        .withAddress("A1:Z10")
        .build())
    .visibleView().rows()
    .buildRequest()
    .get();

```