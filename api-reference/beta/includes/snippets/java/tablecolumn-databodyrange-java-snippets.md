---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c73d8bffc1ea3f3cc41540dacd8daa2c41015dba
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440651"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().tables("{id|name}").columns("{id|name}")
    .dataBodyRange()
    .buildRequest()
    .get();

```