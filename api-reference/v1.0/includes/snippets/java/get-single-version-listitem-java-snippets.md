---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f4acf44e6e67676acb27c4ca0239ed56c643b384
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976418"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("expand", "fields"));

ListItemVersion listItemVersion = graphClient.sites("{site-id}").lists("{list-id}").items("{item-id}").versions("{version-id}")
    .buildRequest( requestOptions )
    .get();

```