---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b26f89990954458f819202eab6f8a92f357b17b62f17ec4107daa8a6b5b3dfbb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101035"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFill workbookRangeFill = new WorkbookRangeFill();
workbookRangeFill.color = "#00FF00";

graphClient.me().drive().items("{id}").workbook().worksheets("{sheet-id}")
    .range(WorkbookWorksheetRangeParameterSet
        .newBuilder()
        .withAddress("$B$1")
        .build()).format().fill()
    .buildRequest()
    .patch(workbookRangeFill);

```