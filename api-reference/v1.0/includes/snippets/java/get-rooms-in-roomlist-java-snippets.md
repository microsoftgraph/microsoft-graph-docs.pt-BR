---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4da35d4e686ea40754a5bd0293c20c5ec89c5b0d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975389"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RoomCollectionPage rooms = graphClient.places("bldg2@contoso.com").microsoft.graph.roomlist().rooms()
    .buildRequest()
    .get();

```