---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f4d18ef824fa24c5e289f1330fa038b47fd847b2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864273"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String sourceData = "sourceData-value";

String seriesBy = "seriesBy-value";

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}")
    .setData(sourceData,seriesBy)
    .buildRequest()
    .post();

```