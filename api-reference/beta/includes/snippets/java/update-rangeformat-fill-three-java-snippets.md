---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d5af592a670aefeeb9fa9ba0e7cebdd901155f0d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976069"
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