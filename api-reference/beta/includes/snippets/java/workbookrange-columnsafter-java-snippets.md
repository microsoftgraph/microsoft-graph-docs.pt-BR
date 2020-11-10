---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 518e6756bb03407791643c4e6f5749d5ff23da86
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980884"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.drive().root().workbook().worksheets("{id}")
    .range()
    .columnsAfter(null)
    .buildRequest()
    .post();

```