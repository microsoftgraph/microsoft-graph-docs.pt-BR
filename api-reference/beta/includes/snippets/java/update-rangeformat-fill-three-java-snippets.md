---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d5af592a670aefeeb9fa9ba0e7cebdd901155f0d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308856"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFill workbookRangeFill = new WorkbookRangeFill();
workbookRangeFill.color = "#0000FF";

graphClient.me().drive().items("{id}").workbook().worksheets("Sheet1")
    .range("$C$1").format().fill()
    .buildRequest()
    .patch(workbookRangeFill);

```