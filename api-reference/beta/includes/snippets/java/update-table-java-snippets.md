---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bc40d2097ab411087d4eebbc099f679bb6ca17544a26865b71e39ff6cd204790
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159338"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookTable workbookTable = new WorkbookTable();
workbookTable.name = "name-value";
workbookTable.showHeaders = true;
workbookTable.showTotals = true;
workbookTable.style = "style-value";

graphClient.me().drive().items("{id}").workbook().tables("{id|name}")
    .buildRequest()
    .patch(workbookTable);

```