---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 449f1b93cb001e3107d7bd68007de4ad8898ab54
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891990"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFill workbookRangeFill = new WorkbookRangeFill();
workbookRangeFill.color = "#0000FF";

graphClient.me().drive().items("{id}").workbook().worksheets("{sheet-id}")
    .range('$C$1').format().fill()
    .buildRequest()
    .patch(workbookRangeFill);

```