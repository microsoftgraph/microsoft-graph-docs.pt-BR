---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d44971533dd923937b3ea89b9a3b3e168f4d9823ebc67143da739ffb6f35988d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103106"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().tables("{id|name}")
    .headerRowRange()
    .buildRequest()
    .get();

```