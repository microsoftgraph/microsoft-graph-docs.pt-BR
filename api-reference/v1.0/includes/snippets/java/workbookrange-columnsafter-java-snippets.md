---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0da01bd0a9a16aef0a7572ba5bef89ead9e1c985b682d22fd2cd36e166a36f3c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275267"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().root().workbook().worksheets("{id}")
    .range()
    .columnsAfter(WorkbookRangeColumnsAfterParameterSet
        .newBuilder()
        .withCount(2)
        .build())
    .buildRequest()
    .get();

```