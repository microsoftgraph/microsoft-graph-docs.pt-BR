---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f743163d0a489b39642a0126a408ecdffb786ece
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983462"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("expand", "fields"));

ListItem listItem = graphClient.sites("{site-id}").lists("{list-id}").items("{item-id}")
    .buildRequest( requestOptions )
    .get();

```