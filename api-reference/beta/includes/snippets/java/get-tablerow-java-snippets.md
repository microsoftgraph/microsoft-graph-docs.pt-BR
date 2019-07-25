---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 102d73224e0d5c3310e91ee31e0ecb06655b6eb9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35868556"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookTableRow workbookTableRow = graphClient.me().drive().items("{id}").workbook().tables("{id|name}").rows("{index}")
    .buildRequest()
    .get();

```