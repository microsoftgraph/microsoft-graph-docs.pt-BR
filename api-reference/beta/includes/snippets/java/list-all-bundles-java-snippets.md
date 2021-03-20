---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 22b8c6b37625603d2de620bb1e7281e9c9d671f7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977892"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItemCollectionPage bundles = graphClient.drive().bundles()
    .buildRequest()
    .get();

```