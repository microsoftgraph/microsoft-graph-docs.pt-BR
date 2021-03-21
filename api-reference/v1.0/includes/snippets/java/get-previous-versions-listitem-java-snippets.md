---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9b385054b5d79f51c9b1903d812e4c60d67ef77d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970166"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ListItemVersionCollectionPage versions = graphClient.sites("{site-id}").lists("{list-id}").items("{item-id}").versions()
    .buildRequest()
    .get();

```