---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 37244fa9352f2b55b0e0deb3d95ada348f922661
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972989"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemEmailCollectionPage emails = graphClient.me().profile().emails()
    .buildRequest()
    .get();

```