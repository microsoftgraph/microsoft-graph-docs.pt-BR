---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: be5f1da1de69478d130a0a4651ecab5acb6a33f6dfe414de6ead70f35acbcb7a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899795"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.domains("contoso.com")
    .buildRequest()
    .delete();

```