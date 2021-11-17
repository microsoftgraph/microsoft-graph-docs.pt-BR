---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3537e44c864b49be578c04fb1c088c690ad79ea16f3b290f36ee117ac64244d2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214608"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonInterestCollectionPage interests = graphClient.me().profile().interests()
    .buildRequest()
    .get();

```