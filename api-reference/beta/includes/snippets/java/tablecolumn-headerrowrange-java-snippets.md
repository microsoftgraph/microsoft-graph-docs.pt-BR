---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6094393508617b5bbaa2331a670e5b5c9d9bbd30d2a83584a70de2b867328551
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216845"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().tables("{id|name}").columns("{id|name}")
    .headerRowRange()
    .buildRequest()
    .get();

```