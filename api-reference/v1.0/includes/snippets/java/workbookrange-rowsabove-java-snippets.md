---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bf885bafd89ed309e3e0224e50fce2e9bb0f0737
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/16/2021
ms.locfileid: "49882812"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().root().workbook().worksheets("{id}")
    .range()
    .rowsAbove(2)
    .buildRequest()
    .get();

```