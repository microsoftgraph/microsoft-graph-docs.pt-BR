---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ca250405c1528b972b78a272bf068ef0c497702e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981220"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItemCollectionPage following = graphClient.me().drive().following()
    .buildRequest()
    .get();

```