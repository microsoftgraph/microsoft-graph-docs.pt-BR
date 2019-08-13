---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 448f69ccf688fe5c9e1cdb7347311105f8e62d92
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324740"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFill workbookRangeFill = new WorkbookRangeFill();
workbookRangeFill.color = "#00FF00";

graphClient.me().drive().items("{id}").workbook().worksheets("{sheet-id}")
    .range("$B$1").format().fill()
    .buildRequest()
    .patch(workbookRangeFill);

```