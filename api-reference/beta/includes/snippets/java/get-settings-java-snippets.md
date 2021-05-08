---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fbaebf6de77f3fbdf69825f3b975652cb1b17c3d
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240862"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Settings settings = graphClient.compliance().ediscovery().cases("5b840b94-f821-4c4a-8cad-3a90062bf51a").settings()
    .buildRequest()
    .get();

```