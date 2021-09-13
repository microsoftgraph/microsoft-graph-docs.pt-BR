---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b64005dd48777c7619c12384767a7e2f0a80eed79d4c0a486e88c3ff9c52ba7d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101037"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFill workbookRangeFill = new WorkbookRangeFill();
workbookRangeFill.color = "#0000FF";

graphClient.me().drive().items("{id}").workbook().worksheets("{sheet-id}")
    .range(WorkbookWorksheetRangeParameterSet
        .newBuilder()
        .withAddress("$C$1")
        .build()).format().fill()
    .buildRequest()
    .patch(workbookRangeFill);

```