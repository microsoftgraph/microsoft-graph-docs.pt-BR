---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 40d8f2fc72a5c55d6840433fb85352f0218a1ab2
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/16/2021
ms.locfileid: "49882953"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.drive().root().workbook().worksheets("{id}")
    .range()
    .columnsBefore(2)
    .buildRequest()
    .get();

```