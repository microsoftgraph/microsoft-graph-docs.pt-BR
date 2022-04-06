---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 22b8c6b37625603d2de620bb1e7281e9c9d671f7
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757884"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItemCollectionPage bundles = graphClient.drive().bundles()
    .buildRequest()
    .get();

```