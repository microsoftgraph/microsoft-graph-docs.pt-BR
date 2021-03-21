---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 307c8f7557553ad56cd4aa30b6e4da53d2fe4881
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980081"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalConnectionCollectionPage connections = graphClient.external().connections()
    .buildRequest()
    .get();

```