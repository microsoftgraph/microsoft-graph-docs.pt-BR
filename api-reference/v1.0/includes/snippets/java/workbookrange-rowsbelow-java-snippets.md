---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 39f57d272709c9cf32697560cf70ee252d09f765
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/16/2021
ms.locfileid: "49882778"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().root().workbook().worksheets("{id}")
    .range()
    .rowsBelow(2)
    .buildRequest()
    .get();

```