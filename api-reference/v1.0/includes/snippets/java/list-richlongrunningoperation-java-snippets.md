---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 561e704dfae1a5344e9be64a6446c5580e71440d
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65314199"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

List list = graphClient.sites("root").lists("Documents")
    .buildRequest()
    .get();

```