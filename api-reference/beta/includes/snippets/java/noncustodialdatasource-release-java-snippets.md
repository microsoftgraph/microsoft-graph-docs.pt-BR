---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fa7244087bee074276fbba32457e8b95af863de9
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240895"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.compliance().ediscovery().cases("5b840b94-f821-4c4a-8cad-3a90062bf51a").noncustodialDataSources("8e402dd7f3c94a3abc086e5d07db1c6d")
    .release()
    .buildRequest()
    .post();

```