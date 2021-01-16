---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e30db702183135a145ea806df4cf213c319c258b
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883134"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().root().workbook().worksheets("{id}")
    .range()
    .columnsAfter(2)
    .buildRequest()
    .get();

```