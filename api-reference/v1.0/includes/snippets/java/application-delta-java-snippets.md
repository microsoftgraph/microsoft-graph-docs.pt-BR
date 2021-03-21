---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2e9640a3bea143bf0c6bf36e64e8cc9d31e8c4cb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977535"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ApplicationDeltaCollectionPage delta = graphClient.applications()
    .delta()
    .buildRequest()
    .get();

```