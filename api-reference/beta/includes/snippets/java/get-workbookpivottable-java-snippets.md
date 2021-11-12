---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5952a7ffd8e5c8eb80bbbd13e7f6b7cacf92e07d47071556917efdf5703aa00c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157353"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookPivotTable workbookPivotTable = graphClient.drive().root().workbook().worksheets("{id}").pivotTables("{id}")
    .buildRequest()
    .get();

```