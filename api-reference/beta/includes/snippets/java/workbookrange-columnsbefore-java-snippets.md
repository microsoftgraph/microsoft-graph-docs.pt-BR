---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c7116e7aca0ad93dd8a596bedf186392736bae8b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972716"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.drive().root().workbook().worksheets("{id}")
    .range()
    .columnsBefore(WorkbookRangeColumnsBeforeParameterSet
        .newBuilder()
        .withCount(2)
        .build())
    .buildRequest()
    .get();

```