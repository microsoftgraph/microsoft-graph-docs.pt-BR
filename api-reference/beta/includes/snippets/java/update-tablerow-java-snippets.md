---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3d3fe94d99a23f0c72bca3f2fa3bac95c30eaa8cb0c277a2deb43d51cb49c0a8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216147"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookTableRow workbookTableRow = new WorkbookTableRow();
workbookTableRow.index = 99;
workbookTableRow.values = JsonParser.parseString("\"values-value\"");

graphClient.me().drive().items("{id}").workbook().tables("{id|name}").rows("{index}")
    .buildRequest()
    .patch(workbookTableRow);

```