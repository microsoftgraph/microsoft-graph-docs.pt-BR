---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8ea4edf39e4b8571e3fe14f6b6acbb2670311626
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65208680"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.sites("root").lists("Documents").items("2").documentSetVersions("1")
    .buildRequest()
    .delete();

```