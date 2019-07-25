---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: de1d3377e7eb89d12bcc57e85670eece3dad9a65
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889839"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFill workbookRangeFill = new WorkbookRangeFill();
workbookRangeFill.color = "color-value";

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range().format().fill()
    .buildRequest()
    .patch(workbookRangeFill);

```