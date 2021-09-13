---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c0dee3631202098ffc714d602f3c635c42b6aae314f26b3b060fef83157b94d3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329971"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}")
    .range()
    .buildRequest()
    .get();

```