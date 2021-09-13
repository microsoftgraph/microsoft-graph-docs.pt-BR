---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ef7aa6725adeb95597f6c95029c3314bd972223a29d5fb4712b29cee00c10725
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275733"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}")
    .range(WorkbookWorksheetRangeParameterSet
        .newBuilder()
        .withAddress("A1:B2")
        .build())
    .buildRequest()
    .get();

```