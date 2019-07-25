---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c21a7adfd2090732a5976e645773b8d787ea7b50
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881122"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String color = "color-value";

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").format().fill()
    .setSolidColor(color)
    .buildRequest()
    .post();

```