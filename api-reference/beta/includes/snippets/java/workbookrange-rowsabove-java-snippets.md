---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: acb9977573ba72de28553bbe5a2597e1924d9a4d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866326"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.drive().root().workbook().worksheets("{id}")
    .range()
    .rowsAbove(count)
    .buildRequest()
    .post();

```