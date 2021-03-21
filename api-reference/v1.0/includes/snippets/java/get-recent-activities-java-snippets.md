---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 91307029fb4d4c2eff5f9a329b282fd4c9712ef7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970105"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserActivityRecentCollectionPage recent = graphClient.me().activities()
    .recent()
    .buildRequest()
    .get();

```