---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 381820ffda5d6c302a27638f5d0ffa4ca3373e6c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975064"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TrendingCollectionPage trending = graphClient.me().insights().trending()
    .buildRequest()
    .get();

```