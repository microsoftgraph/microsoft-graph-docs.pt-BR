---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e32b62cb2084c8bb0772c99247dc87b6c470359b
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210682"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonNameCollectionPage names = graphClient.me().profile().names()
    .buildRequest()
    .get();

```