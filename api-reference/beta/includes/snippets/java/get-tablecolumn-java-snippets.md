---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d80228fcc1c15f7fa5ee2da0c981aa94320d997b051a246c17cdbb4d5d4db98d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57376572"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookTableColumn workbookTableColumn = graphClient.me().drive().items("{id}").workbook().tables("{id|name}").columns("{id|name}")
    .buildRequest()
    .get();

```