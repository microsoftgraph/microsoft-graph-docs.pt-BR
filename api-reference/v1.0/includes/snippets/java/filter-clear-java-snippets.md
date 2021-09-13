---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 43be041c195a016368810e8ac6b66fa7bc48b432b2f6c586853af629eef49438
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327905"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().tables("{id|name}").columns("{id|name}").filter()
    .clear()
    .buildRequest()
    .post();

```