---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ba627bfbba0bdd558e921aa50b8e4bc6cb4a5375
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866443"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.drive().root().workbook().worksheets("{id}").pivotTables("{id}")
    .refresh()
    .buildRequest()
    .post();

```