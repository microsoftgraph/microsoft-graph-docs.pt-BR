---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 38352edb5b502f610cc5a399f92c96b87f1edafe46bcf61c0de69d488d1171c7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215367"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnenoteOperation onenoteOperation = graphClient.me().onenote().operations("{id}")
    .buildRequest()
    .get();

```