---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 31e4341abb0c0821485694acea3cdc45503a509d052e8948fbb64d180ef2edef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275636"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintOperation printOperation = graphClient.print().operations("{printOperationId}")
    .buildRequest()
    .get();

```