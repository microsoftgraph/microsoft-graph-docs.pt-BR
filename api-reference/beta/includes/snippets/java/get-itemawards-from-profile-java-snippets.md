---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 98c96701c59b5e7e7b2b3026f64b0e83f0650edc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975222"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonAwardCollectionPage awards = graphClient.me().profile().awards()
    .buildRequest()
    .get();

```