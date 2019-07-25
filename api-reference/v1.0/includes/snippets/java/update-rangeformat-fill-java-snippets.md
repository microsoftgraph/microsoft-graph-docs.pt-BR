---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 82361b81701421c6f1270c911848c87e6f874864
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891981"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFill workbookRangeFill = new WorkbookRangeFill();
workbookRangeFill.color = "#FF0000";

graphClient.me().drive().items("{id}").workbook().worksheets("{sheet-id}")
    .range('$A$1').format().fill()
    .buildRequest()
    .patch(workbookRangeFill);

```