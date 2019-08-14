---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 495452d16cbfbecd640057bbd512bdace1635eec
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372680"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFill workbookRangeFill = new WorkbookRangeFill();
workbookRangeFill.color = "#00FF00";

graphClient.me().drive().items("{id}").workbook().worksheets("Sheet1")
    .range("$B$1").format().fill()
    .buildRequest()
    .patch(workbookRangeFill);

```