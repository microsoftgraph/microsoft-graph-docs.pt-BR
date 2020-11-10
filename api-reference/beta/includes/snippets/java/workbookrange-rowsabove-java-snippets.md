---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 304822fcd166f57cc0b59871ff33c8bbec35df01
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977097"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.drive().root().workbook().worksheets("{id}")
    .range()
    .rowsAbove(null)
    .buildRequest()
    .post();

```