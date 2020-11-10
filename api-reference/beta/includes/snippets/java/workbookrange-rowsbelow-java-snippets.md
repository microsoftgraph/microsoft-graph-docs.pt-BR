---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 17e973eeddbb2362ba67a860bce9b3e1357aaf03
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977084"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.drive().root().workbook().worksheets("{id}")
    .range()
    .rowsBelow(null)
    .buildRequest()
    .post();

```