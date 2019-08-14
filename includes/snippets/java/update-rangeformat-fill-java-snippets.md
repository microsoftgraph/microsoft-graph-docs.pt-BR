---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f065e3009ddeaef637f5aa6f7ae03e4fe1e9e870
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372674"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFill workbookRangeFill = new WorkbookRangeFill();
workbookRangeFill.color = "#FF0000";

graphClient.me().drive().items("{id}").workbook().worksheets("Sheet1")
    .range("$A$1").format().fill()
    .buildRequest()
    .patch(workbookRangeFill);

```