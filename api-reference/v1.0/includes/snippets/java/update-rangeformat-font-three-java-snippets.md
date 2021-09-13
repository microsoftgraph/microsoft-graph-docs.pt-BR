---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 37e813d0e2d641b215b9472fdcbbc6ba8b65b113ef4c21b5f5a260ae081e26e0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101036"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFont workbookRangeFont = new WorkbookRangeFont();
workbookRangeFont.underline = "Single";
workbookRangeFont.color = "#FFFFFF";
workbookRangeFont.size = 26d;

graphClient.me().drive().items("{id}").workbook().worksheets("{sheet-id}")
    .range(WorkbookWorksheetRangeParameterSet
        .newBuilder()
        .withAddress("$C$1")
        .build()).format().font()
    .buildRequest()
    .patch(workbookRangeFont);

```