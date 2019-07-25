---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 95967356be14262d0d099548ce59acafd55540a5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886611"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookTableColumn workbookTableColumn = graphClient.me().drive().items("{id}").workbook().tables("{id|name}").columns("{id|name}")
    .buildRequest()
    .get();

```